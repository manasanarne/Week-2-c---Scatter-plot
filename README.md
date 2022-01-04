
Names <- c("Varsha","Saswitha","Manasa","Pragna","Sreya")
> Rollno <- c("Y20CS124","Y20CS135","Y20CS110","Y20CS093","Y20CS176")
> Gender <- c("Female","Female","Female","Female","Female")
Marks <-c(9,3,6,8,9)
Fee <-c(69400,57892,58903,69400,67390)
Section <-c("B","C","B","B","C")

rvrstudents <-data.frame(Names,Rollno,Gender,Marks,Fee,Section)
rvrstudents
write.csv(rvrstudents,"Rvr_Students.csv",row.names=F)

a <- read.csv("Rvr_Students.csv")



plot(rvrstudents$Fee,
     rvrstudents$Marks,
     main="RVRJCCE",
     xlab="students fee",
     ylab="students marks",
     col="blue",
     las=1)
cor(rvrstudents$Fee,rvrstudents$Marks)

OUTPUT:
> Names <- c("Varsha","Saswitha","Manasa","Pragna","Sreya")
> Rollno <- c("Y20CS124","Y20CS135","Y20CS110","Y20CS093","Y20CS176")
> Gender <- c("Female","Female","Female","Female","Female")
> Marks <-c(9,3,6,8,9)
> Fee <-c(69400,57892,58903,69400,67390)
> Section <-c("C","C","C","B","B")
> rvrstudents <-data.frame(Names,Rollno,Gender,Marks,Fee,Section)
> rvrstudents
     Names     Rollno    Gender   Marks   Fee     Section
1   Varsha    Y20CS134   Female     9    69400       B
2   Saswitha  Y20CS145   Female     3    57892       C
3   Manasa    Y20CS149   Female     6    58903       B
4   Pragna    Y20CS127   Female     8    69400       B
5   Sreya     Y20CS129   Female     9    67390       C
> write.csv(rvrstudents,"Rvr_Students.csv",row.names=F)
> a <- read.csv("Rvr_Students.csv")
> plot(rvrstudents$Fee,
+      rvrstudents$Marks,
+      main="RVRJCCE",
+      xlab="students fee",
+      ylab="students marks",
+      col="blue",
+      las=1)
> cor(rvrstudents$Fee,rvrstudents$Marks)
[1] 0.8986413
