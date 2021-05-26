# Matplotlib
### Matplotlib is a Python package for 2D-graphics. It provides both a very quick way to visualize data from Python and publication-quality figures in many formats.
### pyplot provides a convenient interface to the matplotlib object-oriented plotting library.
### Figures, Subplots, Axes and Ticks
### A **Figure** in matplotlib is the whole window in the user interface. **Subplot** positions the plots in a regular grid and **Axes** allows free placement within the figure. when calling plot, matplotlib calls gca() to get the current axes and gca in turn calls gcf() to get the current figure. If there is none it calls figure() to make one, strictly speaking, to make a subplot(111). **Ticks** are an important part of publishing-ready figures. Matplotlib provides a totally configurable system for ticks. 
### Animation matplotlib can be done