# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# ATE (Average Treatment Effectin) percentage points under subgroup heterogeneity (post-estimation) Use ate_pct With (in) R Software
install.packages("remotes")
remotes::install_github("zengying17/ate_pct-r")
library("sandwich")
library("atepct")
# Estimate ATE (Average Treatment Effectin) percentage points under subgroup heterogeneity (post-estimation) Use ate_pct With (in) R Software
ate_pct_r = read.csv("https://raw.githubusercontent.com/timbulwidodostp/ate_pct_r/main/ate_pct_r/ate_pct_r.csv", sep = ";")
lm <- lm(lny ~ x + gr1 + gr2 + gr3, data = ate_pct_r)
ate_pct <- ate_pct(lm, c("gr1","gr2","gr3"))
ate_pct
summary(ate_pct)
# ATE (Average Treatment Effectin) percentage points under subgroup heterogeneity (post-estimation) Use ate_pct With (in) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished