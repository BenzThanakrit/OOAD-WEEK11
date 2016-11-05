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

#code 
```
@startuml
title decode
[*] -> ready
ready -> decodeing 
decodeing  -> ready   :decodeing complete
decodeing -> decodeing :decodeing not complete
@enduml.
```
![](http://www.plantuml.com/plantuml/img/LOvB2iCm44FtSmhj2eNc05sKtADquNgcnM1xWgCiSlj-0dMw4HhfCMYS6HgNakMWzWXBfj0dq75tqWiqDOjCNeM9sQ0MNKsknnjE5pGBkifNF-TMflg4TFlZ09nx7BrCsMWxyk_33gtEZijeLT-3XnS0)

#Activity1
```
code gade
@startuml
(*) --> "Initialization"

if "point >79" then
  -->[true] "gade A"
  --> "Transcript"

else
  ->[false] if "point >69" then
    -->[true] "gade B"
      --> "Transcript"
else
     ->[false]if "point >59" then 
     -->[true] "gade C"
       --> "Transcript"
     else
     ->[false]if "point >49" then 
     -->[true] "gade D"
       --> "Transcript"
endif
"Transcript" --> (*)

@enduml
```
![](http://www.plantuml.com/plantuml/img/VT4z3u9030RWlR-YwQGcR7x4XU37ukv662vofqtEWnnbyTTx8CPBGBRcRViCRTQ8yj8-BInMIqoI5EdYM5XPVYdXoX406wIwOYUOxlQ4yj0Ei9lDnRUwGBghKkE1FY7IrIlNt3pN4fQrRNJNI7EZGbbWf6r_sjWxKXzFc0E9aHgXcm55m2dsz6N7Rf_Eu-jv_FmVrwva0t7KpuIh0sIX6Lxm1W00)
