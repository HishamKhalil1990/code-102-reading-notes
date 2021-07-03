# React 4
## Dynamic Routes
### Page Path Depends on External Data
#### Each page path depends on external data. Next.js allows you to statically generate pages with paths that depend on external data. This enables dynamic URLs in Next.js.
### How to Statically Generate Pages with Dynamic Routes
#### To create dynamic routes for blog posts:
- Each post should have the path `/posts/<id>`, where `<id>` is the name of the markdown file under the top-level posts directory.
- Since having `ssg-ssr.md` and `pre-rendering.md`, then the paths are `/posts/ssg-ssr` and `/posts/pre-rendering`.
![ex](https://i.ibb.co/hy8vV9S/1.jpg)
### Implement getStaticPaths
#### To implement then:
- Create a file called `[id].js` inside the `pages/posts` directory.
- Remove `first-post.js` inside the `pages/posts` directory
- Open `pages/posts/[id].js` in your editor and paste the following code:
```
import Layout from '../../components/layout'

export default function Post() {
  return <Layout>...</Layout>
}
```
- Open `lib/posts.js` and add the following getAllPostIds function at the bottom. It will return the list of file names `excluding .md` in the `posts` directory
- Import the `getAllPostIds` function and use it inside `getStaticPaths`. Open `pages/posts/[id].js` and copy the following code above the exported Post component:
```
import { getAllPostIds } from '../../lib/posts'

export async function getStaticPaths() {
  const paths = getAllPostIds()
  return {
    paths,
    fallback: false
  }
}
```
### Implement getStaticProps
#### To implement then:
- Open `lib/posts.js` again and add the following `getPostData` function at the bottom. 
- Open pages/posts/[id].js and replace this line `import { getAllPostIds } from '../../lib/posts'` eith:
```
import { getAllPostIds, getPostData } from '../../lib/posts'

export async function getStaticProps({ params }) {
  const postData = getPostData(params.id)
  return {
    props: {
      postData
    }
  }
}
```
- Update the Post component to use postData. In `pages/posts/[id].js` replace the exported `Post` component with the following code:
```
export default function Post({ postData }) {
  return (
    <Layout>
      {postData.title}
      <br />
      {postData.id}
      <br />
      {postData.date}
    </Layout>
  )
}
```
### Render Markdown
#### To render markdown content, we’ll use the remark library which we can install by `npm install remark remark-html` then import `import remark from 'remark'` and `import html from 'remark-html'` and update the `getPostData()` function in the same file as follows to use `remark`:
```
export async function getPostData(id) {
  const fullPath = path.join(postsDirectory, `${id}.md`)
  const fileContents = fs.readFileSync(fullPath, 'utf8')

  // Use gray-matter to parse the post metadata section
  const matterResult = matter(fileContents)

  // Use remark to convert markdown into HTML string
  const processedContent = await remark()
    .use(html)
    .process(matterResult.content)
  const contentHtml = processedContent.toString()

  // Combine the data with the id and contentHtml
  return {
    id,
    contentHtml,
    ...matterResult.data
  }
}
```
### Dynamic Routes Details
#### Some essential information you should know about dynamic routes:
- Fetch External API or Query Database:
    - Like `getStaticProps`, `getStaticPaths` can fetch data from any data source.
- Development v.s. Production
    - In development `npm run dev or yarn dev`, `getStaticPaths` runs on every request.
    - In production, `getStaticPaths` runs at build time.
- Catch-all Routes:
    - Dynamic routes can be extended to catch all paths by adding three dots (...) inside the brackets
- Router:
    - If you want to access the `Next.js` router, you can do so by importing the useRouter hook from `next/router`.
## Deploying Your Next.js App
### The easiest way to deploy Next.js to production is to use the Vercel platform developed by the creators of Next.js. Vercel is an all-in-one platform with Global CDN supporting static & JAMstack deployment and Serverless Functions. We believe Vercel is the optimal place to deploy Next.js apps.
### You can use default values for the following settings — no need to change anything —. Vercel automatically detects that you have a Next.js app and chooses optimal build settings for you:
* Project Name
* Root Directory
* Build Command
* Output Directory
* Development Command
