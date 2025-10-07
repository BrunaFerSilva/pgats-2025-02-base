# 🧪 Testes Automatizados - Projeto Original

## ✅ **8 Testes Criados com Sucesso!**

Este arquivo contém os 8 testes automatizados para o projeto [BrunoM-Nascimento/pgats-02-api](https://github.com/BrunoM-Nascimento/pgats-02-api).

## 📊 **Resultados dos Testes**

- **✅ 8 testes criados**
- **✅ 8 testes passando** 
- **✅ 0 testes falhando**
- **✅ 100% de sucesso!** 🎉

## 🚀 **Como executar os testes**

### 1. **Instalar dependências**
```bash
npm install
```

### 2. **Executar os testes**
```bash
# Rodar todos os testes
npm test

# Rodar testes em modo watch (recomendado para desenvolvimento)
npm run test:watch

# Rodar todos os testes (incluindo futuros)
npm run test:all
```

## 🧪 **O que cada teste faz?**

### **POST /transfers - Criar Transferência**

1. **✅ Sucesso** - Cria transferência com dados corretos (código 201)
2. **✅ Erro de validação** - Falta dados obrigatórios (código 400)
3. **✅ Erro de validação** - Valor é zero (código 400)
4. **✅ Erro de autenticação** - Sem token (código 401)
5. **✅ Erro de autenticação** - Token inválido (código 401)

### **GET /transfers - Listar Transferências**

6. **✅ Sucesso** - Lista transferências com token válido (código 200)
7. **✅ Erro de autenticação** - Sem token (código 401)
8. **✅ Erro de autenticação** - Token inválido (código 401)

## 📁 **Arquivos criados**

```
projeto/
├── test/
│   └── transfer.test.js          # 8 testes de transferências
├── .mocharc.json                 # Configuração do Mocha
├── package.json                  # Scripts e dependências atualizados
└── TESTES_README.md              # Esta documentação
```

## 🔧 **Dependências adicionadas**

```json
{
  "devDependencies": {
    "chai": "^4.3.10",
    "mocha": "^10.2.0", 
    "supertest": "^6.3.3"
  }
}
```

## 📝 **Scripts do package.json**

```json
{
  "scripts": {
    "test": "mocha test/transfer.test.js --timeout 10000",
    "test:all": "mocha test/**/*.test.js --timeout 10000",
    "test:watch": "mocha test/transfer.test.js --watch --timeout 10000"
  }
}
```

## 🎯 **Tecnologias usadas**

- **Mocha** - Framework de testes
- **Chai** - Biblioteca de asserções  
- **SuperTest** - Testes de API HTTP
- **JWT** - Autenticação com tokens

## 💡 **Como os testes funcionam**

1. **Setup**: Cria tokens válidos e inválidos antes dos testes
2. **Teste de Sucesso**: Envia dados corretos + token válido
3. **Teste de Validação**: Testa campos obrigatórios e regras de negócio
4. **Teste de Autenticação**: Verifica se a API bloqueia acesso sem token
5. **Verificação**: Confirma códigos de status e mensagens de erro

## 🚀 **Próximos passos**

- ✅ **Testes funcionando** - Pronto para usar!
- 🔄 **Adicionar mais testes** - Para outros endpoints
- 📊 **Relatórios** - Configurar relatórios de cobertura
- 🔄 **CI/CD** - Integrar com GitHub Actions

## 📚 **Documentação do projeto original**

Consulte o [README.md](https://github.com/BrunoM-Nascimento/pgats-02-api) do projeto original para entender a API completa.

---

**🎉 Parabéns! Seus testes automatizados estão funcionando perfeitamente!**
