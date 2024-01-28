**Instalar Git en su Ultima Version En Debian 11**


**Instalas git como usuario root** :
1.Ejecuta estos comandos como usuario root:

```bash
sudo su
```
```bash
sudo apt install git
```

Una vez ayas instalado Git vuelve al usuario normal con el siguien comando:```bash
exit```
**Listo continua con los pasos**
*********

1. **Añadir ruta al perfil del usuario:**
   Ejecuta estos comandos como usuario normal:

   ```bash
   echo 'export PATH="/usr/local/bin:$PATH"' >> ~/.bashrc
   source ~/.bashrc
   ```

2. **Verificar la ruta de ejecución de Git:**
   Ejecuta el siguiente comando como usuario normal:

   ```bash
   echo $PATH
   ```

   Asegúrate de que `/usr/local/bin` esté en la lista.

3. **Alias para git:**
   Agrega el alias como usuario normal:

   ```bash
   echo 'alias git="/usr/local/bin/git"' >> ~/.bashrc
   source ~/.bashrc
   ```

Después de realizar estos pasos como usuario normal, intenta nuevamente ejecutar `git --version`. Si el problema persiste, verifica si hay mensajes de error específicos.