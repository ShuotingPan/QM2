# QM2
!mkdir data
     

!mkdir data/wk2
!curl https://s3.eu-west-2.amazonaws.com/qm2/wk2/incomes.csv -o ./data/wk2/incomes.csv
     
  

import pandas
import pylab
import matplotlib.pyplot as plt
# make the plots a little wider by default
%matplotlib inline
plt.style.use('ggplot')

pylab.rcParams['figure.figsize'] = (10., 8.)
     

data_path = "./data/wk2/incomes.csv"

income =  pandas.read_csv(data_path, index_col=0)
income.head()
