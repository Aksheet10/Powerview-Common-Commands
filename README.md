# PowerView

---

https://github.com/PowerShellEmpire/PowerTools/blob/master/PowerView/powerview.ps1

Save this in a notepad as `PowerView.ps1`

---

Open Command Promt as administrator

`powershell -ep bypass`

`. .\PowerView.ps1`

`Get-NetDomain` - Information about the domain

![Pasted image 20210529193905](https://user-images.githubusercontent.com/71016915/120078710-74c81e00-c0ce-11eb-8e99-77bccf25cced.png)

---

`Get-NetDomainControllers` - Get all the domains

![Pasted image 20210529194115](https://user-images.githubusercontent.com/71016915/120078721-801b4980-c0ce-11eb-80b5-4e71a717bc0b.png)

---

`Get-DomainPolicy`

![Pasted image 20210529194318](https://user-images.githubusercontent.com/71016915/120078729-84dffd80-c0ce-11eb-90f1-376086a97f4b.png)

---

`Get-NetUser` / `Get-DomainUser` - Both are similar

![image](https://user-images.githubusercontent.com/71016915/120273307-f2a54880-c2cb-11eb-8300-f67722c9117b.png)

![Pasted image 20210529194934](https://user-images.githubusercontent.com/71016915/120078738-8c9fa200-c0ce-11eb-88ef-fe929b2c3118.png)

---

`Get-DomainUser  -Properties cn,description` is same as `Get-NetUser | select cn, description`

![Pasted image 20210529200230](https://user-images.githubusercontent.com/71016915/120078753-a4772600-c0ce-11eb-9950-9a8dec644ecb.png)

---

`Get-NetComputer`

![image](https://user-images.githubusercontent.com/71016915/120272915-6d219880-c2cb-11eb-97d7-45cd47b4d56c.png)

---

`Get-NetUser "name"` is same as `Get-DomainUser "name"`

![image](https://user-images.githubusercontent.com/71016915/120272805-44999e80-c2cb-11eb-86dd-f45076e0b8e6.png)

![Pasted image 20210529213314](https://user-images.githubusercontent.com/71016915/120078762-ae008e00-c0ce-11eb-8da0-549b65fcde39.png)

---

`Get-NetGroupMember "Domain Admins"`

![Pasted image 20210529215827](https://user-images.githubusercontent.com/71016915/120078819-de482c80-c0ce-11eb-8b76-00567dfa3005.png)

---

`Get-NetGroup` - Get all the groups

`Get-NetGroup "Domain Admins"` - Gets specific group

![image](https://user-images.githubusercontent.com/71016915/120105515-db087b80-c176-11eb-8fbf-8e6aba0ecac5.png)

---

 `Get-DomainComputer | select cn, dnshostname` also same as `Get-NetComputer | select cn, dnshostname`
 
 ![image](https://user-images.githubusercontent.com/71016915/120272915-6d219880-c2cb-11eb-97d7-45cd47b4d56c.png)


![Pasted image 20210529220504](https://user-images.githubusercontent.com/71016915/120078823-e86a2b00-c0ce-11eb-844b-b8f77dc6899c.png)

 ---
 
 `Invoke-ShareFinder` - Shows all the shares
 
 ![Pasted image 20210529221344](https://user-images.githubusercontent.com/71016915/120078828-ed2edf00-c0ce-11eb-8a95-5642a33a9a54.png)
 
 ---
 
  `Get-NetComputer -Properties samaccountname` same as `Get-DomainComputer -Properties samaccountname`
  
  ![image](https://user-images.githubusercontent.com/71016915/120273599-592a6680-c2cc-11eb-83d0-872548fa0205.png)

  ---
  
`Get-NetGPO -Properties displayname,whenchanged` same as `Get-DomainGPO -Properties displayname, whenchanged`
 
 ![image](https://user-images.githubusercontent.com/71016915/120091377-3d865b00-c128-11eb-8765-238bccf07bd5.png)\
 
 ![image](https://user-images.githubusercontent.com/71016915/120274659-c8ed2100-c2cd-11eb-92a2-efc3061d55a8.png)

 
 
