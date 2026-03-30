# Implementations

## v0.1.1 — 2026-03-30

- Menu de contexto do Windows: "Converter DNG → JPG" e "Converter DNG → PNG" no clique-direito
- Modo CLI com argparse: subcomandos `convert`, `install`, `uninstall`
- Busca recursiva em subpastas (CLI por padrão, GUI via checkbox)
- Extração da lógica de conversão para funções standalone (`load_dng`, `convert_file`, `find_dng_files`)
- Registro no Windows via `winreg` (HKCU, sem precisar de admin)

## v0.1.0 — 2026-03-30

- App desktop para conversão DNG → JPG/PNG com interface tkinter
- Seleção por pasta ou arquivos individuais
- Escolha de formato (JPG/PNG) com controle de qualidade JPG
- Conversão em cascata: rawpy → Pillow (TIFF) → ImageMagick (subprocess)
- Barra de progresso e log em tempo real
- Conversão em thread separada (GUI não trava)
- Arquivo salvo ao lado do original com mesmo nome
