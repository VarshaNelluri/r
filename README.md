# week1a-barplot
Names <- c("MANYA","SUBHIKSHA","SHIVA","KIRAN","SATWIKA")
Rollno <- c("Y20CS126","Y20CS127","Y20CS128","Y20CS129","Y20CS130")
Gender <- c("FEMALE","FEMALE","MALE","MALE","FEMALE")
Marks <-c(9,9,8,9,7)
Fee <-c(69400,57892,58903,69400,67390)
Section <-c("B","B","C","B","C")

rvrstudents <-data.frame(Names,Rollno,Gender,Marks,Fee,Section)
rvrstudents
write.csv(rvrstudents,"Rvr_Students.csv",row.names=F)

a <- read.csv("Rvr_Students.csv")


barplot(rvrstudents$Marks,
        xlab="Students names",
        ylab="marks",
        main="RVRJCCE",
        xlim=c(1,10),
        ylim=c(1,10),
        col="pink",
        names.arg=rvrstudents$Names,
        las=2)



OUTPUT:
> Names <- c("MANYA","SUBHIKSHA","SHIVA","KIRAN","SATWIKA")
> Rollno <- c("Y20CS126","Y20CS127","Y20CS128","Y20CS129","Y20CS130")
> Gender <- c("FEMALE","FEMALE","MALE","MALE","FEMALE")
> Marks <-c(9,9,8,9,7)
> Fee <-c(69400,57892,58903,69400,67390)
> Section <-c("B","B","C","B","C")
> rvrstudents <-data.frame(Names,Rollno,Gender,Marks,Fee,Section)
> rvrstudents
      Names   Rollno Gender Marks   Fee Section
1     MANYA Y20CS126 FEMALE     9 69400       B
2 SUBHIKSHA Y20CS127 FEMALE     9 57892       B
3     SHIVA Y20CS128   MALE     8 58903       C
4     KIRAN Y20CS129   MALE     9 69400       B
5   SATWIKA Y20CS130 FEMALE     7 67390       C
> write.csv(rvrstudents,"Rvr_Students.csv",row.names=F)
> a <- read.csv("Rvr_Students.csv")
> barplot(rvrstudents$Marks,
+         xlab="Students names",
+         ylab="marks",
+         main="RVRJCCE",
+         xlim=c(1,10),
+         ylim=c(1,10),
+         col="pink",
+         names.arg=rvrstudents$Names,
+         las=2)
> 
