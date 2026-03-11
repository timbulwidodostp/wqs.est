# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Weighted Quantile Sum Regression Use wqs.est (wqs) With (In) R Software
install.packages("remotes")
remotes::install_github("cran/wqs")
library("wqs")
# Estimate Weighted Quantile Sum Regression Use wqs.est (wqs) With (In) R Software
wqs.est = read.csv("https://raw.githubusercontent.com/timbulwidodostp/wqs.est/main/wqs.est/wqs.est.csv", sep = ";")
y.train <- wqs.est[,'y']
x.train <- wqs.est[,-10]
wqs.est <- wqs.est(y.train, x.train, B = 10)
head(wqs.est$q.train, 1)
head(wqs.est$wts.matrix, 1)
wqs.est$weights
head(wqs.est$WQS, 1)
wqs.est$fit
# Weighted Quantile Sum Regression Use wqs.est (wqs) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished