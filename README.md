# Nova AI Web

Frontend público experimental da Nova AI.

**Atenção:** este repositório não contém o Qwen3-4B nem chaves de API. O site depende de um gateway Cloudflare Worker autenticado que aciona o workflow em [Nova-AI](https://github.com/raphaelsancho21-byte/Nova-AI) (privado).

Para publicar: **Settings → Pages → Build and deployment → Deploy from a branch → main → /(root) → Save**.

Depois de instalar o gateway, atualize `config.js` com a URL pública do Worker (nunca coloque tokens no frontend).

GitHub Actions não é servidor 24h: cada resposta aciona uma execução temporária com custo de minutos e latência significativa. O acesso por chave compartilhada é adequado somente para uso restrito; para uso público é necessário autenticação individual e limites por usuário.
