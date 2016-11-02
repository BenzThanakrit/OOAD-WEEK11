# OOAD-WEEK11
State Diagram
#code 
```
@startuml

title  Glass 
[*] --> GlassEmpty

GlassFull : Water
GlassFull --> [*]
@enduml
```
![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuU8goIp9ILLGSCz9B2vMu8hMYbNGrRM3S5rp2qegkRWGR0MOZ5jfJWuNdALWfH2UM99QX2G2CWDe5XSNbqDgNWhG8W00)

#code turn on computer
```
@startuml

title Turn On
[*] -> off
off -> on :swict is turn on
on -> boot : swict on computer

boot -> ready : booting computer
ready -> [*]
@enduml
```

![](http://www.plantuml.com/plantuml/img/HOun2eH034NxdEBNWXUmMBp1DdPYuUgu36Yop6HOlBrVBIm2oNyFyjliO_AohI8UVGteIbAyLVfgGFs2BOjmhbNHv7-S7373JyrK619zp1mDRifeikrNF2Iv08KKndcdSTvHluzm0nhy9stGcLKE)

#code shut down
```
@startuml
title shut down
[*] -> ready
ready -> off :swict is turn off
off -> [*]
@enduml
```
![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuU8goIp9ILKepYWjKKZ9By_ZYjQALT2rKoXAJKofv0AJ86v-Mfg2LN5vPdA9GcQnGabfKHv8Y0ia39G5wk5oICrB0He80000)

#code instruction
```
@startuml

title read instruction
[*] -> ready
ready -> reading :instruction coming
reading -> reading :reading not complete
reading -> sending :reading complete
sending -> sending : sending not complete
sending -> ready :sending complete

@enduml
```
![](http://www.plantuml.com/plantuml/img/LSyn2e0m30NGFQV8B7W11-azn44qIA6cqiR1srkLb7GfwSyZ92xBakGw0e1u2OI9bWqzPqdNAZuoJDsC_VZbDtolVZtlE1YAQpnA1jgpJ0kEyh8pa925cRY55Md7eberuupyznmqgGHSISgr3m00)
