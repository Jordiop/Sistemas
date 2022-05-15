# Actividad 3 Sistemas Informáticos

### Introducción

Lo primero que he hecho, es actualizar todos los archivos de ayuda que vienen con powershell debido a que estaban desactualizados y no mostraban toda la información. El comando usado es `update help`

#### Task 1: Use "Get-Help" to find out more information about 5 cmdlets.

`get-help new-item`

![imatge](https://user-images.githubusercontent.com/95173613/160280791-a5d934d9-7585-4ea6-a42a-399437273b93.png)

`get-help move-item`

![imatge](https://user-images.githubusercontent.com/95173613/160280808-99968587-4815-4250-944b-5e11648027df.png)

`get-help get-alias`

![imatge](https://user-images.githubusercontent.com/95173613/160280821-e1e838ab-ba24-4c29-ad9c-760aff7fba6f.png)

`get-help rename-item`

![imatge](https://user-images.githubusercontent.com/95173613/160280994-ec2608bd-7a7f-4b15-bab9-50803bf3cbf3.png)

`get-help set-item`

![imatge](https://user-images.githubusercontent.com/95173613/160281016-0aa5c3c5-b414-465d-a499-edd7316fc322.png)

---

#### Task 2: Use “Get-Help” with the “–Example” parameter for the 5 cmdlets you discovered more about in task 1.

`get-help new-item -example`

![imatge](https://user-images.githubusercontent.com/95173613/160281546-78cf91b8-0f43-406a-a0fc-434740419079.png)


`get-help move-item -example`

![imatge](https://user-images.githubusercontent.com/95173613/160281563-690b0e4c-2c29-4d94-a285-2a591c37ebca.png)


`get-help get-alias -example`

![imatge](https://user-images.githubusercontent.com/95173613/160281581-e714735f-2433-4cd0-84ae-bb3883cba63a.png)


`get-help rename-item -example`

![imatge](https://user-images.githubusercontent.com/95173613/160281600-33d6f6ee-bdf9-4210-8ffc-7d818e64ad5d.png)


`get-help set-item -example`

![imatge](https://user-images.githubusercontent.com/95173613/160281650-baa3bd51-a894-4d07-af6a-efb419c56765.png)

---

#### Task 3. Create a new text file named “TestFile.txt” under C:\Maximo\PowerShell\Workshop1\%USERNAME%

```
md C:\Maximo\PowerShell\Workshop1\jordiop | New-item -Path C:\Maximo\PowerShell\Workshop1\jordiop -Name Testfile.txt -ItemType File
```

#### Task 4. Populate the text file you created in task 3 with all three datatypes we’ve covered: “Boolean”, “String” and “Int”

![imatge](https://user-images.githubusercontent.com/95173613/160282018-27a06606-474b-402e-8d2b-e0705c3c9dd4.png)

![imatge](https://user-images.githubusercontent.com/95173613/160282023-3a15e3e8-38d3-42c1-b6ad-881d68e9ec41.png)

#### Task 5. Read from the text file and use “Get-Member” to find the datatype returned

![imatge](https://user-images.githubusercontent.com/95173613/160282234-cfb17d6e-941c-449e-a22a-434bb32e7fd8.png)

#### Task 6. Overwrite all data within the text file that you created in task 3.

`set-content -path C:\Maximo\PowerShell\Workshop1\jordiop\testfile.txt -value "Un 10"`

#### Task 7. Format the data returned by a cmdlet into a list

![imatge](https://user-images.githubusercontent.com/95173613/160494893-b27452af-1b39-4602-ade6-7ea0ce2d07d5.png)

#### Task 8. Pipe "Get-command" into "Out-GridView"

![imatge](https://user-images.githubusercontent.com/95173613/160284437-c6e22235-3797-4e5a-855d-f7aa9cb966e3.png)

#### Task 9. Pipe the 5 cmdlets you discovered in taskk 1 into "out-gridview"

![imatge](https://user-images.githubusercontent.com/95173613/160482775-56bf5e23-5935-44b1-84eb-e7af2d3069b8.png)

![imatge](https://user-images.githubusercontent.com/95173613/160482892-86180624-704a-44c1-b62f-9b40ca105ced.png)

![imatge](https://user-images.githubusercontent.com/95173613/160483028-ef201992-cd43-4477-9458-05b18869609f.png)

![imatge](https://user-images.githubusercontent.com/95173613/160483113-a06a92ac-a153-4568-b534-ff7244c43816.png)

![imatge](https://user-images.githubusercontent.com/95173613/160483164-b0800f82-d714-450c-bb9a-48af5e42f4fc.png)

#### Task 10. Find the official PowerShell documentation library from Microsoft

![imatge](https://user-images.githubusercontent.com/95173613/160483335-5518dfdc-00d0-4def-9cb5-dd4d8ac5bdca.png)

https://docs.microsoft.com/es-es/powershell/


29 de Març
