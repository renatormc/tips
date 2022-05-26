
# Instalar Windows 11

Inicie a instalação do Windows normalmente  
Quando lhe for apresentada uma tela dizendo que sua máquina é incompatível pressione Shift + F10 para abrir o prompt de comando.  
Digite regedit.exe e pressione Enter;

Vá até HKEY_LOCAL_MACHINE\SYSTEM\Setup e crie uma nova chave com o nome LabConfig.  
Na chave LabConfig, crie duas novas entradas:

BypassTPMCheck = dword: 00000001
BypassSecureBootCheck = dword: 00000001
salve as alterações e volte uma etapa e prossiga novamente.
