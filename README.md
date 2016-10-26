# OOAD-WEEK10
Sequence Diagram
##ส่งการบ้าน Sequence Diagram นายเอกชัย ภมรสุขนิรันดิ์ 57030253
#Sequence Diagram เรื่องที่1 การโทรหากัน
...
person1 -> phone1:PressTheNumber
phone1 -> person1:ShowDisPlayNumber
person1 -> phone1:PressTheCallButton
phone1 -> phone2:SignalCallphone2
phone2 -> phone2:WaitRecipient
phone2 -> phone1:acceptance
phone1 -> person1:acceptancephone2
phone2 -> person2:AnswerTheTelephone
person2 -> person1:talk
person1 -> person2:EndAConversation
person1 -> phone1:HangUp
phone1 -> phone2:SignaHangUp
phone2 -> person2:PpressHangUp
...
![](http://www.plantuml.com/plantuml/img/TP313e8m44JlVWK_u84UUp11DF5aY60yhtK3ZNNRj4NYtmiK8uZSkZklavarQ9scE5fl8bDfmfXd5fqhAZpMZolQLTZsUa1vNkbc9rscuFLX5arIK6fRUwzfRDIz6CzbIQ0w8Ym2mKR41QG_eP168lbVEUOW11eF9F1FogyuT-yHnXDo3TesPO4gK4CJDZRoeEwJXiFlFTsILDEp7S7Bhk3i2WUWycmMce_5IQpCTCSByXi0)

#Sequence Diagram เรื่องที่2 สั่งซื้อสินค้าในเว็บ
...
purchaser -> WebProducts:web access
purchaser -> WebProducts:SelectProducts
WebProducts -> purchaser:ShowProducts
purchaser -> WebProducts:OrderProducts
WebProducts -> Salesman:TransmissionOrder
Salesman -> Salesman:SalesmanPhipment
Salesman -> purchaser:TransmissionProductsMail
...
![](http://www.plantuml.com/plantuml/img/TOvD2eGm34RtFKKlC1VemXl821rm7MEWXVwHLBo-ADJHHNS9t_jUKZP61qAiFuEUQPauhnjMCJij6X19H9KUOoaGrhQgHtIITyrOb_URwjg-l1BtP1O2IOHaVWn9eXVnELqDrQ8NreR9-H8frHVr_-nfQ-T6yE40)


#Sequence Diagram เรื่องที่3 โอนเงินในตู้ATM
...
TransFerMomey -> ATMMachine:InsertTheCard
ATMMachine -> monitor:ShowSlotID
TransFerMomey -> Keyboard:EnterATD
Keyboard -> ATMMachine:SendItToTheMachine
ATMMachine -> Server:IDIsCorrect?
Server -> ATMMachine:IDBeCorect
ATMMachine -> monitor:ShowMenu
TransFerMomey -> Keyboard:PressMenuMoneyTransFer
Keyboard -> ATMMachine:DataTransFer
TransFerMomey -> Keyboard:OK
Keyboard -> ATMMachine:SendData
ATMMachine -> Server:No/Yes
Server -> ATMMachine:Yes
ATMMachine -> monitor:ShowYes
Server -> Addressee:SebeMoneyToAddressee
Server -> ATMMachine:TellYourBalance
ATMMachine -> Printer:PrinterBalance
Printer -> TransFerMomey:Bill
ATMMachine -> TransFerMomey:ATMCardBack
...
![](http://www.plantuml.com/plantuml/img/VPB1QiCm38RlUOg-mEZTXusctY0KTuNuqgER_90mrmBPNSdRpwP9HqsIax7qwPT-ovgDyrzWHLSCcxVtpKuhPPgkTn2Ly-2WE-mDjyL_8c5NSdqW5dL7zzfIg6IXSwa3XWl5Kl7f0dYdPJ55iaOrN5i5JR7L6CgwrU1ViAXavVV4Z2Py58zOFh8i4Oa8hCohu6uhqvuOtYT6aSCmSKkpInFCaraM_JwicKyYyvQFj3t3pvjDYMMNMLdR9bj8_IvuEADdS5vVmzeptRWqrhWctyc9-xHMCPuJD5uJyV8QekojpIHUWPXB7wqqpSyV)


#Sequence Diagram เรื่องที่4 เข้าเล่นเกมHON
...
Person -> KerboardAndMouse:PressProgramGarena
KerboardAndMouse -> ProgramGarena:SendDataProgramGarena
ProgramGarena -> Monitor:ShowProgramGarena
Person -> KerboardAndMouse:PressID
KerboardAndMouse -> ProgramGarena:SendDataID
ProgramGarena -> Monitor:ShowID
Person -> KerboardAndMouse:Enter
KerboardAndMouse -> ProgramGarena:CheckDataID
ProgramGarena -> Server:HaveUsersOfThis?
Server -> ProgramGarena:TheHaveUsers
ProgramGarena -> Monitor:ShowGamesMenu
Person -> KerboardAndMouse:PressGamesHON
KerboardAndMouse -> ProgramGarena:SelectGamesHON
ProgramGarena -> GamesHON:OpenGamesHON
GamesHON -> Monitor:ShowGamesHON
GamesHON -> Server:ViewDataAllGamesHON
Server -> GamesHON:ReceiveDataAllGamesHON
GamesHON -> Monitor:SendDataToTheMonitor
Person -> KerboardAndMouse:PressKerboardAndMouse
KerboardAndMouse -> GamesHON:SelectMenuGamesHON
GamesHON -> Server:SendDataToServer
Server -> GamesHON:SendDataToGamesHON
...
![](http://www.plantuml.com/plantuml/img/bP71Se8m54NtVeK_q1_8GiUH3dGw25FGVGhNmeX9vmNmzqi4mX0Hx0vUpkFU74AGacBzjbb_WhubftGdKbzM2YmaA1MI_25-TJb1y9NDwBqHmIA8rE4b7--DtlIIBqLUIc9H9cyMkb3em_b7YmQUZTRdp_FUHGbw8MsV8RayYuj0DOXvlCPHDLd1ESvojLsryyUFnHaCEr_UvLSe7w9QT7OdlU3maha2IMaM7Whq9opuXJ1O_p1PqGOw8wSSDorjLnG66wIOd2yao6lOv6HYzzTZsKZiXejkxEca8zEcrQEbprrjAD8EfkurCFte3m00)

#Sequence Diagram เรื่องที่5 เติมเงินโทรศัพท์มือถือ
...
Person -> KerboarMenuCall:PressMenuCall
KerboarMenuCall -> Machine:SensDataToMachine
Machine -> Monitor:ShowMenuCall
Person -> KerboarMenuCall:PressPrepaidCard
KerboarMenuCall -> Machine:DataTOTheMachine
Machine -> Monitor:ShoePrepaidCard
Person -> KerboarMenuCall:PressCall
KerboarMenuCall -> Machine:Call
Machine -> Server:SendPrepaidCard
Server -> Server:AddAmountMoney
Server -> Machine:SendDataToMenuMessage
MenuMessage -> Monitor:ShowMessageRefill
...
![](http://www.plantuml.com/plantuml/img/XP3D3S8m38NldQ8Bi40EI5MveOgATW633OqKOkIa8BOd3GKYaD9BVlniV_PhIHpRShKkjoG71cd8ZZKOereXvzw_uaUT2Xeu3jgIwiYw3NZeUOuKynsJs6hFehg1xvzcRHuQZYjeh44mnutCNJzG7ajfkmNoqgfHJp0ToOraSW1JoYkS95I8rOL7wyDSz4Zqn4ESFGpO9em2vx3Gz_tlPGplwQIDUG80)

README.md 
md เป็นภาษา Markdown นิยมใช้ใน wiki ของ github 

ตัวอย่างโค้ด
```
# Heading ระดับ 1 
## Heading ระดับ 2
### Heading ระดับ 3
 
```

ผลที่ได้
# Heading ระดับ 1 
## Heading ระดับ 2
### Heading ระดับ 3


## Code ภาษาซี

ตัวอย่างโค้ด
<pre>
  ``` c
  #include <stdio.h>
  Main()
  {
     Printf("Hello");
  }
  ```
</pre> 
ผลที่ได้
  ``` c
  #include <stdio.h>
  Main()
  {
     Printf("Hello");
  }
  ```
 
