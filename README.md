# Redes sem Fio — Apresentações em LaTeX/Beamer + TikZ

Conversão das apresentações originais em PDF (Profa. Anelise Munaretto) para
**LaTeX Beamer** com diagramas **TikZ**, conteúdo atualizado a 2026 e novas aulas.

## Estrutura

```
.
├── aula1.pdf … aula6.pdf      # PDF originais (não modificados)
├── latex/
│   ├── preamble.tex           # preâmbulo comum (tema, cores, estilos TikZ)
│   ├── aula1.tex … aula12.tex # aulas convertidas + novas aulas
│   └── aula1.pdf … aula12.pdf # PDF gerados
└── docs/
    └── informe_melhorias.pdf   # informe de melhorias
```

## Como compilar

Requer `tectonic`:

```bash
cd latex
make              # compila todas as 12 aulas + informe
```

ou manualmente:

```bash
tectonic aula1.tex   # … até aula12.tex
```

## Conteúdo das aulas

| Aula | Tema | Destaques 2026 |
|------|------|----------------|
| 1 | Internet: revisão (caps. 1–6 Kurose) | IPv6, SDN, QUIC, Wireshark renovado |
| 2 | Introdução às redes sem fio | Wi-Fi 6/6E/7, 5G NR, WPA3 |
| 3 | Roteamento ad hoc | AODV, DSR, TBRPF, OLSR, MANET RFCs |
| 4 | Protocolos MAC | TDMA/FDMA, ALOHA, CSMA/CD/CA, 802.11e/ax |
| 5 | Redes emergentes | LPWAN, 5G, NTN, LEO, Wi-Fi 7, MLO |
| 6 | Qualidade de Serviço (QoS) | Intserv/Diffserv, RSVP, QOLSR, FTS |
| 7 | **5G e redes móveis** | SA/NSA, SBA, mMIMO, mmWave, slicing, 5G-Advanced, 6G |
| 8 | **IoT sem fio e LPWAN** | LoRaWAN, Sigfox, NB-IoT, LTE-M, MQTT, CoAP |
| 9 | **Redes veiculares** | C-V2X vs 802.11p, NR-V2X, platooning, simulação |
| 10 | **Drones, satélites e NTN** | FANET, LEO (Starlink), 3GPP NTN, handover |
| 11 | **IA e ML nas redes** | RL, DQN, LSTM para alocação, handover, beamforming |
| 12 | **Segurança em redes sem fio** | WPA2/WPA3, KRACK, LoRaWAN security, 5G AKA |

## Notas

- Idioma: português brasileiro (pt-BR).
- Os PDF originais (`aula1-6.pdf`) permanecem intactos na raiz.
- Requer `tectonic` ≥ 1.0 (funciona também com `pdflatex`).