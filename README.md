# Sistema de Gerador de Notas Fiscais com Controle de Acesso

## Descrição
Sistema completo para geração de notas fiscais com controle de acesso baseado em planos pagos via Pix.

## Funcionalidades Implementadas

### ✅ Acesso Inicial Gratuito
- Usuário pode gerar até 5 notas fiscais gratuitamente
- Após usar as 5 notas, o sistema bloqueia automaticamente
- Exibe modal com planos pagos

### ✅ Planos Pagos com QR Code Pix
- **Plano 50 notas (30 dias)** - R$ 59,90 → qrcode1.jpg
- **Plano 100 notas (30 dias)** - R$ 89,90 → qrcode2.jpg  
- **Plano Ilimitado (30 dias)** - R$ 250,00 → qrcode3.jpg
- Botão "Copiar Chave Pix" com feedback visual
- Chave Pix copiada automaticamente para clipboard

### ✅ Sistema de Suporte
- Mensagem de suporte aparece após 1 minuto (60 segundos)
- Formulário com campos: Nome, E-mail, Mensagem
- Envio automático para WWWWWWWW@gmail.com
- Confirmação "Mensagem enviada com sucesso!"

### ✅ Sistema de Senhas de Ativação
- 20 senhas exclusivas por plano (não reutilizáveis)
- **Plano 50 notas**: NF50-XXXXXXXX
- **Plano 100 notas**: NF100-XXXXXXXX  
- **Plano Ilimitado**: NFUNL-XXXXXXXX
- Validação automática e ativação do plano
- Controle de expiração (30 dias) e limites

### ✅ Controle de Acesso Inteligente
- Armazenamento em localStorage
- Verificação automática de limites e expiração
- Status visual do plano ativo
- Bloqueio automático quando necessário

## Arquivos Incluídos

1. **nota_fiscal_generator_complete.html** - Sistema completo integrado
2. **qrcode1.jpg** - QR Code para Plano 50 notas
3. **qrcode2.jpg** - QR Code para Plano 100 notas  
4. **qrcode3.jpg** - QR Code para Plano Ilimitado
5. **README.md** - Esta documentação

## Como Usar

1. Extraia todos os arquivos na mesma pasta
2. Abra o arquivo `nota_fiscal_generator_complete.html` no navegador
3. O sistema está pronto para uso!

## Senhas de Teste

### Plano 50 Notas (Exemplos):
- NF50-A1B2C3D4
- NF50-E5F6G7H8
- NF50-I9J0K1L2

### Plano 100 Notas (Exemplos):
- NF100-X1Y2Z3A4
- NF100-B5C6D7E8
- NF100-F9G0H1I2

### Plano Ilimitado (Exemplos):
- NFUNL-Z1A2B3C4
- NFUNL-D5E6F7G8
- NFUNL-H9I0J1K2

## Configurações Importantes

### E-mail de Suporte
Atualmente configurado para: **WWWWWWWW@gmail.com**
Para alterar, edite a linha no código:
```javascript
const mailtoLink = `mailto:WWWWWWWW@gmail.com?subject=Suporte - Ativação de Plano&body=${emailBody}`;
```

### Chaves Pix
As chaves Pix nos botões são exemplos genéricos. Para usar em produção, substitua pelos códigos Pix reais nos atributos `data-pix` dos botões.

## Recursos Técnicos

- **Armazenamento**: localStorage do navegador
- **Validação**: CPF, CNPJ, CEP com APIs externas
- **Geração PDF**: Biblioteca jsPDF
- **Responsivo**: Design adaptável para mobile
- **Segurança**: Senhas únicas não reutilizáveis

## Suporte

Para dúvidas ou problemas, entre em contato através do formulário integrado no sistema ou pelo e-mail configurado.

---

**Desenvolvido com todas as funcionalidades solicitadas integradas ao código original.**

