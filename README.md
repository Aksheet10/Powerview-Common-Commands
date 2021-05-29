# PowerView

---

`powershell -ep bypass`

`. .\PowerView.ps1`

`Get-NetDomain` - Information about the domain

![Pasted image 20210529193905](https://user-images.githubusercontent.com/71016915/120078710-74c81e00-c0ce-11eb-8e99-77bccf25cced.png)


`Get-NetDomainControllers` - Get all the domains

![Pasted image 20210529194115](https://user-images.githubusercontent.com/71016915/120078721-801b4980-c0ce-11eb-80b5-4e71a717bc0b.png)


![Pasted image 20210529194318](https://user-images.githubusercontent.com/71016915/120078729-84dffd80-c0ce-11eb-90f1-376086a97f4b.png)

`Get-DomainPolicy`

`Get-NetUser` / `Get-DomainUser`

![Pasted image 20210529194934](https://user-images.githubusercontent.com/71016915/120078738-8c9fa200-c0ce-11eb-88ef-fe929b2c3118.png)


`Get-DomainUser  -Properties description,pwdlastset,cn`

`Get-NetUser | select cn, description`

![Pasted image 20210529200230](https://user-images.githubusercontent.com/71016915/120078753-a4772600-c0ce-11eb-9950-9a8dec644ecb.png)


`Get-NetComputer`

![Pasted image 20210529211029](https://user-images.githubusercontent.com/71016915/120078759-a9d47080-c0ce-11eb-96ec-cb62f5c804d6.png)


`Get-DomainUser "name"`

![Pasted image 20210529213314](https://user-images.githubusercontent.com/71016915/120078762-ae008e00-c0ce-11eb-8da0-549b65fcde39.png)



`Get-NetGroupMember "Domain Admins"`

![Pasted image 20210529215827](https://user-images.githubusercontent.com/71016915/120078819-de482c80-c0ce-11eb-8b76-00567dfa3005.png)


`Get-NetGroup`

![Pasted image 20210529220504](https://user-images.githubusercontent.com/71016915/120078823-e86a2b00-c0ce-11eb-844b-b8f77dc6899c.png)

 
 `Get-DomainComputer | select cn, dnshostname`
 
 `Invoke-ShareFinder`
 
 ![Pasted image 20210529221344](https://user-images.githubusercontent.com/71016915/120078828-ed2edf00-c0ce-11eb-8a95-5642a33a9a54.png)
 
 ![Pasted image 20210529221932](https://user-images.githubusercontent.com/71016915/120078834-ef913900-c0ce-11eb-8070-fe3232a3e91e.png)

  
 `Get-NetComputer -Properties samaccountname`
 
