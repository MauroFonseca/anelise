# Redes sem Fio — Presentacións en LaTeX/Beamer + TikZ

Conversión das presentacións orixinais en PDF (Profa. Anelise Munaretto) a
**LaTeX Beamer** con diagramas **TikZ**, contido actualizado a 2026 e proposta
de novas aulas.

## Estrutura

```
.
├── aula1.pdf … aula6.pdf      # PDF orixinais (sen modificar)
├── latex/
│   ├── preamble.tex           # preámbulo común (tema, cores, estilos TikZ)
│   ├── aula1.tex … aula6.tex  # aulas convertidas a Beamer + TikZ
│   └── aula1.pdf … aula6.pdf  # PDF xerados
└── docs/
    └── informe_melloras.tex   # informe de melloras + proposta de novas aulas
    └── informe_melloras.pdf
```

## Como compilar

Requírese `tectonic` (auto-descarga de paquetes):

```bash
cd latex
make              # compila aula1..6 e o informe
```

ou manualmente:

```bash
tectonic aula1.tex   # … até aula6.tex
tectonic ../docs/informe_melloras.tex
```

## Contido das aulas

| Aula | Tema | Novidades 2026 |
|------|------|----------------|
| 1 | Internet: revisión (caps. 1–6 Kurose) | IPv6, SDN/OpenFlow, QUIC, Wireshark actualizado |
| 2 | Introdución ás redes sen fío | Wi-Fi 6/6E/7, 5G NR, WPA3 |
| 3 | Roteamento ad hoc (AODV, DSR, TBRPF, OLSR) | RFCs orixinais, comparativa |
| 4 | Protocolos MAC (ALOHA, CSMA/CD/CA, 802.11) | CSMA/CD histórico, 802.11e/ax |
| 5 | Redes emerxentes | **reescrita**: LPWAN, 5G, NTN, LEO, Wi-Fi 7, MLO |
| 6 | Calidade de servizo (QoS) | Intserv/Diffserv, RSVP, 802.11e, QOLSR/FTS |

Vexa `docs/informe_melloras.pdf` para o detalle de melloras e as **6 novas
aulas propostas** (5G, IoT/LPWAN, VANET, NTN, IA, seguridade).

## Notas

- Idioma: galego (coherente co material orixinal).
- Os PDF orixinais (`aula*.pdf`) mantéñense intactos na raíz.
- Precisase `tectonic` ≥ 1.0 (tamén funciona con `pdflatex`).