![Logo do pacote](assets/logo.png){ width="300" .center }
# Resumos Anpuh

## Como usar?

Você pode chamar as escalas via linha de comando. Por exemplo:

```bash
poetry run escalas
```

Retornando os graus e as notas correspondentes a essa escala:

```bash
┏━━━━┳━━━━┳━━━━━┳━━━━┳━━━━┳━━━━┳━━━━━┓
┃ I  ┃ II ┃ III ┃ IV ┃ V  ┃ VI ┃ VII ┃
┡━━━━╇━━━━╇━━━━━╇━━━━╇━━━━╇━━━━╇━━━━━┩
│ D# │ F  │ G   │ G# │ A# │ C  │ D   │
└────┴────┴─────┴────┴────┴────┴─────┘
```

### Alteração na escala

O primeiro parâmetro do CLI é a tônica da escala que deseja exibir. Desta forma, você pode chamar a escala de Fá sustenido, por exemplo, da seguinte forma:

```bash
poetry run escalas F#
```

Retornando:

```bash
┏━━━━┳━━━━┳━━━━━┳━━━━┳━━━━┳━━━━┳━━━━━┓
┃ I  ┃ II ┃ III ┃ IV ┃ V  ┃ VI ┃ VII ┃
┡━━━━╇━━━━╇━━━━━╇━━━━╇━━━━╇━━━━╇━━━━━┩
│ F# │ G# │ A#  │ B  │ C# │ D# │ F   │
└────┴────┴─────┴────┴────┴────┴─────┘
```

### Alteração na tonalidade da escala

Você também pode alterar a tonalidade da escala. Esse é o segundo parâmetro da linha de comando. Por exemplo, você pode chamar a escala de Ré sustenido maior.

```bash
poetry run escalas D# menor
```

Retornando:

```bash
┏━━━━┳━━━━┳━━━━━┳━━━━┳━━━━┳━━━━┳━━━━━┓
┃ I  ┃ II ┃ III ┃ IV ┃ V  ┃ VI ┃ VII ┃
┡━━━━╇━━━━╇━━━━━╇━━━━╇━━━━╇━━━━╇━━━━━┩
│ D# │ F  │ G   │ G# │ A# │ C  │ D   │
└────┴────┴─────┴────┴────┴────┴─────┘
```

## Mais informações sobre o CLI

Para descobrir outras opções voce pode usar a flag `--help`:

```bash
poetry run escalas --help
```

Retornando:

```bash
Usage: escalas [OPTIONS] [TONICA] [TONALIDADE]                                          
                                                                                         
╭─ Arguments ───────────────────────────────────────────────────────────────────────────╮
│   tonica          [TONICA]      Tônica da escala [default: C]                         │
│   tonalidade      [TONALIDADE]  Tonalidade da escala [default: maior]                 │
╰───────────────────────────────────────────────────────────────────────────────────────╯
╭─ Options ─────────────────────────────────────────────────────────────────────────────╮
│ --install-completion        [bash|zsh|fish|powershell|p  Install completion for the   │
│                             wsh]                         specified shell.             │
│                                                          [default: None]              │
│ --show-completion           [bash|zsh|fish|powershell|p  Show completion for the      │
│                             wsh]                         specified shell, to copy it  │
│                                                          or customize the             │
│                                                          installation.                │
│                                                          [default: None]              │
│ --help                                                   Show this message and exit.  │
╰───────────────────────────────────────────────────────────────────────────────────────╯
```