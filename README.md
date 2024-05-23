 <p align="center">
<img src="https://cwmkt.com.br/wp-content/uploads/2024/04/logo_github.png" width="240" />
<p align="center">Seja bem-vindo ao Guia de atualização de rebuilds 🚀</p>
</p>
  
<p align="center"> 
<a href="https://hubconnect.top" target="_blank">👉 Participe da Comunidade HubConnect 👈</a>
</p>

<hr />
<hr />

  <details>
<summary>Para individualizar conversas entre agentes</summary>

```bash
mv /home/chatwoot/chatwoot/app/javascript/dashboard/components/ChatList.vue /home/chatwoot/chatwoot/app/javascript/dashboard/components/ChatList.vue.old
```

```bash
cd /home/chatwoot/chatwoot/app/javascript/dashboard/components
```

```bash
wget "https://raw.githubusercontent.com/cwmkt/quepasa/main/ChatList.vue"
```

Após alterações acima, rebuildar seu Chatwoot

```bash
sudo -i -u chatwoot
cd chatwoot
```

```bash
rake assets:precompile RAILS_ENV=production
```

```bash
exit
```

```bash
systemctl daemon-reload && systemctl restart chatwoot.target
```

</details>


  
