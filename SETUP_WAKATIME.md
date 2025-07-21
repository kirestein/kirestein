# 📊 Configurando WakaTime para Estatísticas Reais

Para ter dados reais de desenvolvimento no seu README, siga estes passos:

## 🚀 Passo 1: Criar conta no WakaTime

1. Acesse [wakatime.com](https://wakatime.com)
2. Crie uma conta gratuita
3. Acesse suas configurações para obter a API Key

## 🔧 Passo 2: Instalar o plugin no seu editor

### VS Code
1. Instale a extensão "WakaTime"
2. Cole sua API Key quando solicitado

### Outros editores
- [IntelliJ/PyCharm](https://wakatime.com/intellij)
- [Sublime Text](https://wakatime.com/sublime-text)
- [Vim](https://wakatime.com/vim)
- [Atom](https://wakatime.com/atom)

## 🔐 Passo 3: Configurar secrets no GitHub

1. Vá para `Settings` > `Secrets and variables` > `Actions`
2. Adicione os seguintes secrets:
   - `WAKATIME_API_KEY`: Sua chave da API do WakaTime
   - `GH_TOKEN`: Token do GitHub com permissões de escrita

## ⏱️ Passo 4: Aguardar coleta de dados

- O WakaTime precisa de alguns dias para coletar dados suficientes
- As estatísticas serão atualizadas automaticamente no README
- O workflow roda diariamente às 18:30 UTC

## 📈 Resultado

Após a configuração, você verá estatísticas reais como:

```text
TypeScript   12 hrs 30 mins  ████████████████░░░░░░░░░   45.2%
Python       8 hrs 15 mins   ███████████░░░░░░░░░░░░░░   29.8%
JavaScript   4 hrs 45 mins   ██████░░░░░░░░░░░░░░░░░░░   17.1%
CSS          2 hrs 10 mins   ███░░░░░░░░░░░░░░░░░░░░░░    7.9%
```

## 🔧 Troubleshooting

- **Não aparece dados**: Verifique se a API Key está correta
- **Workflow falha**: Verifique se os secrets estão configurados
- **Dados antigos**: O cache pode levar até 24h para atualizar

## 📚 Recursos Úteis

- [Documentação WakaTime](https://wakatime.com/help)
- [GitHub Actions WakaTime](https://github.com/anmol098/waka-readme-stats)
- [Troubleshooting Guide](https://github.com/anmol098/waka-readme-stats/blob/master/README.md#troubleshooting)