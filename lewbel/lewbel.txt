# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Identification using heteroscedasticity Use lewbel (ivlewbel) With (In) R Software
install.packages("remotes")
remotes::install_github("cran/ivlewbel")
library("ivlewbel")
lewbel = read.csv("https://raw.githubusercontent.com/timbulwidodostp/lewbel/main/lewbel/lewbel.csv",sep = ";")
# Estimation Identification using heteroscedasticity Use lewbel (ivlewbel) With (In) R Software
lewbel_1 <- lewbel(formula = y2 ~ y1 | x1 + x2 | x1 + x2, data = lewbel)
lewbel_1$coef.est
lewbel_1$j.test
lewbel_1$f.test.stats
lewbel_2 <- lewbel(formula = y2 ~ y1 | x1 + x2 | x1 + x2 | z1, data = lewbel)
lewbel_2$coef.est
lewbel_2$j.test
lewbel_2$f.test.stats
# Identification using heteroscedasticity Use lewbel (ivlewbel) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished