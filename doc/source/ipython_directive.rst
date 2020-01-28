
.. ipython:: python
    :suppress:

    import matplotlib.pyplot as plt
    plt.style.use('ggplot')


====================
Ipython  direcitives
====================


Ipython can be invoked with  ``.. ipython:: python``



.. ipython:: python

    import pandas as pd
    import numpy as np




.. ipython:: python

    ts = pd.Series(np.random.randn(1000), index=pd.date_range('1/1/2000', periods=1000))
    ts = ts.cumsum()

    @savefig series_plot_basic.png
    ts.plot()
