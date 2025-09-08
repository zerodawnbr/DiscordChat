# Envio de mensagens do chat

As mensagens digitadas no chat do servidor DayZ são automaticamente enviadas para o **Discord**, em tempo real.  
Isso permite acompanhar conversas, moderar e ter registro mesmo fora do jogo.  

---

## Arquivo de configuração

O sistema utiliza o arquivo `config.json`, que fica na pasta:  
$profile:/ZeroDawnBRCoreTools/DiscordChat/


Dentro desse arquivo você pode habilitar ou desabilitar quais mensagens devem ser enviadas.  

---

## Exemplo de configuração

```json
{
    "logDirect": 0,
    "logGlobal": 0,
    "Servers": [
        {
            "id": "1401242642309709876",
            "token": "vWkzQ3LMbqGA9uxdB9mRxqjHOhz5S5n9s6JdBK3ssqLrjBc0mzq1aDaKorgjWIWgDIG9",
            "sendDirect": 1,
            "sendGlobal": 1
        }
    ]
}
```
Explicação dos campos

## Explicação dos campos

| Campo        | Descrição                                                                 | Valor padrão |
|--------------|---------------------------------------------------------------------------|--------------|
| **logDirect**  | Habilita/Desabilita log de mensagens diretas (`0` = desligado, `1` = ligado) | `0`          |
| **logGlobal**  | Habilita/Desabilita log de mensagens globais                           | `0`          |
| **id**         | ID do canal do Discord onde as mensagens serão enviadas                | vazio        |
| **token**      | Token de autenticação para conexão com o bot                           | vazio        |
| **sendDirect** | Envia mensagens diretas para o Discord (`1` = sim, `0` = não)          | `1`          |
| **sendGlobal** | Envia mensagens globais para o Discord (`1` = sim, `0` = não)          | `1`          |



