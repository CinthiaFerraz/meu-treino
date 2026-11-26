# Meu Treino — PWA

Aplicativo web instalável para acompanhar os quatro treinos semanais, registrar cargas por exercício, marcar séries, consultar histórico, visualizar gráficos e usar cronômetro com alerta sonoro/vibração.

## Como testar
1. Extraia o ZIP.
2. Publique a pasta em um serviço de hospedagem estática com HTTPS (por exemplo, GitHub Pages, Netlify ou Vercel).
3. Abra o endereço no Chrome do Android.
4. Use **Instalar app** ou o menu do Chrome → **Instalar aplicativo / Adicionar à tela inicial**.

O PWA e o Service Worker precisam de HTTPS (ou localhost). Abrir `index.html` diretamente como arquivo não habilita instalação nem modo offline.

## Armazenamento e privacidade
- Registros e rascunhos ficam no `localStorage` do navegador, no próprio aparelho.
- Não há conta, servidor ou sincronização na nuvem.
- Use **Histórico → Exportar backup** regularmente. A limpeza dos dados do navegador pode apagar os registros.
- O backup é um arquivo JSON e pode ser importado novamente.

## Observações
- O gráfico mostra a carga registrada ao longo das sessões para o exercício escolhido.
- O mesmo dia e data atualiza o registro existente em vez de duplicá-lo.
- A carga é registrada em kg por exercício; registre a carga total usada no exercício.
- Cronômetro oferece 45, 60 e 90 segundos, com pausar/continuar, zerar, som e vibração quando disponíveis.
