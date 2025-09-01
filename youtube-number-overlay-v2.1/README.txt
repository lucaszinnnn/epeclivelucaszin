YouTube Number Overlay v2.1 — Só o número (OBS) — COM DEBUG
-----------------------------------------------------------
Novidades:
- Corrige leitura quando o YouTube retorna o número como STRING (ex.: "1234").
- Modo DEBUG: ?debug=1 mostra status/erros no cantinho.
- Resolve links tipo https://youtube.com/@canal/live e /channel/UC...:
  • Busca o channelId a partir do @handle e descobre o vídeo AO VIVO atual.

Como usar:
1) Abra index.html, cole o link da live → Gerar link → cole no OBS (Browser Source).
2) Opcional: acrescente &transparent=1, &interval=10, &fontsize=64, &debug=1

API usada (YouTube Data API v3):
- Videos:    videos?part=liveStreamingDetails&id=VIDEO_ID&key=API_KEY
- Channels:  channels?part=id&forHandle=@handle&key=API_KEY
- Search:    search?part=id&channelId=UC...&eventType=live&type=video&key=API_KEY

Sua API key atual: AIzaSy... (oculta no arquivo config.json)
