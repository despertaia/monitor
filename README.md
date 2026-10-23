# Monitor

Alarme do servidor da Desperta.IA. A cada 5 minutos, testa de fora:

- a biblioteca da Banca: `https://banca.despertaia.com.br/v1/catalog`
- a Controladoria: `https://processos.despertaia.com.br/`

Quando um dos dois para de responder (três tentativas seguidas), manda um aviso no celular pelo
[ntfy](https://ntfy.sh). Quando volta, manda outro. Um run vermelho na aba Actions quer dizer
fora do ar naquele momento.

Para mandar um aviso de teste: Actions › Monitor › Run workflow › marque "Mandar um aviso de teste".
