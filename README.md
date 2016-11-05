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
(*) --> "final"

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
![](http://www.plantuml.com/plantuml/img/VT3B3e8m40NG_Np5pQpKX9sFk6dmyGdk28j6Mcs2XRJb_os8iGd8RdBdpbbCxeDqeNlLjDgiaMK2h8sLDHCP3MuROmF4uSW8JsK9VQK8hbCb-24hXHD_Gl3DIUllphGX7glQgtuX2YtZM2BHzZzjwfrvY6VCaKIY9kXkH46OOozVTkeEwJA-NSQl_t5bAwCfZOPEV3PH7fVnysy0)

#code 
```
@startuml
(*) --> "Eatbreakfast"
Eatbreakfast-->Drink water
if Turn On The Game? then 
  -->[yes]Having Fun
  -->Go To Bed
else 
  -->[no]read book
  -->Go To Bed
endif
"Go To Bed" --> (*)
@enduml
```
![](http://www.plantuml.com/plantuml/img/POz12i8m44NtESKdAnLw1IsYrfsRxAIBAPtQq7O2IQfuUqT54LpEVv-PDsNA5FCyZSQOnMg9ebZ3xYataMdeA6Mhu7VMmYvw6N2Zp56Xx-3cA3W9NC-eQE8DSiy2W-UwyvrJVQIhbmiEixp3Ai05RBarF2R-D2NKUgP54yBmrvFMTyRORs9Vhkgi3gLI_U41)

#code
```
@startuml
start

while (go school)  is (Yes)
:study;
:playground;
endwhile (No)

:Go travel;

stop

@enduml
```
![](http://www.plantuml.com/plantuml/img/BOqn3e0W40JxVSMLyWLexEpiBOaGDJazme66tqkCtHOpiwCMdqiz6Ty0dltWICCcfEikmeReK1gMg0PMImtDmIRsRSjIh-0Gh_0xinZ0Ja8b-pkoGszA0iQEz8SN)

#code 
```
@startuml
(*) --> "GPA"

if "" then
  -->[3.0 => GPA] "send acceptance letter"


else
  -> if "else" then
    -->[2.0 => GPA]"send conditional letter"
else
  -> if "else" then
    -->[1.0 => GPA]"send rejection letter"
endif
"send conditional letter" --> (*)
"send acceptance letter" --> (*)
"send rejection letter" -->  (*)
@enduml
```
![](http://www.plantuml.com/plantuml/img/XT1D2y8m30RWUtv5w4c5YHzdopnvtLqyb2x3IksapVw_QGSRJ8R7zasUaDI9JUJXxM6pss9LQLItvge0N8TA8Jyf0ER_-tb_m8j6IH-e4eKMZRNqOHCieITcYj86v1Fb3erPoAz96PtJx8oCxKFhsFN1-CdvgnoNIgGNsQpCXh0ThCueoyhIiBRCek1dGCbBGIsvdF0B)
