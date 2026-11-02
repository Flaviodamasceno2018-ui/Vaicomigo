# VAICOMIGO 5.1 — conexão pública configurada (TESTE)

- Configuração do projeto Supabase existente inserida em `config.js`: URL e **publishable key**, que é pública.
- Não inclui secret key nem service_role.
- `PRODUCTION_MODE` permanece `false`.
- **Atenção:** `backendReady()` no código antigo apenas detecta a presença das credenciais e pode mostrar “conectado” mesmo que tabelas, RLS ou endpoints não estejam funcionando. Essa indicação NÃO comprova operação real.
- Esta versão não implanta SQL, não altera o Supabase e não publica na Netlify.
- Antes de produção: revisar as políticas RLS, autenticação, endpoints e impedir escrita direta de valores/status de corrida no REST do navegador.
- Se você já salvou outro projeto no navegador, remova os valores antigos no painel “Conectar os dois celulares” para usar os valores padrão desta versão.
