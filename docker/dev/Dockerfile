FROM lurd4862/r_py_baseline

RUN R -e 'install.packages("plotly")'
RUN R -e 'install.packages("FactoMineR")'
RUN R -e 'install.packages("factoextra")'
RUN R -e 'install.packages("yardstick")'

RUN conda install twython