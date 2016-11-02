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
