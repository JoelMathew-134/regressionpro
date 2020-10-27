# regressionpro
import matplotlib.pyplot as plt
from scipy import stats

plt.scatter(x,y)
slope,intercept,r,p,std_err=stats.linregess(x,y)

def myfunc(x):
return slope*x+intercept

std_err=list(map(myfunc,x))
plt.plot(x,std_err)

y=myfunc(x)
print(y)
