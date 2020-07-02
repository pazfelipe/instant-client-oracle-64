# Conexão com banco oracle via instant client

# Banco oracle versão 11g

Baixar os arquivos

Instalar o .deb

```
sudo dpkg -i oracle*.deb
```

Criar o diretório `/opt/oracle/`

Rodar o comando 
```
sudo chown -R $USER:$USER /opt/oracle
```

Colocar o arquivo `tnsnames.ora` dentro do diretório criado

Rodar os comandos
```
echo export TNS_ADMIN=”/opt/oracle” >> ~/.bashrc
echo export ORACLE_HOME="/usr/lib/oracle/11.2/client64"  >> ~/.bashrc
echo export PATH=”$PATH:/usr/lib/oracle/11.2/client64/bin” >> ~/.bashrc
echo export LD_LIBRARY_PATH=”/usr/lib/oracle/11.2/client64/lib/” >> ~/.bashrc
source ~/.bashrc
```
Como alternative ao PLSQL (windows), pode ser usado o Dbeaver.
