# 🔧 Compilador - Análise Léxica e Sintática

Implementação completa de um compilador com análise léxica, parser LL(1) e parser SLR(1) para uma linguagem de programação simplificada (estilo C).

## 📋 Características

- ✅ **Analisador Léxico** (Scanner) - Reconhece 40+ tipos de tokens
- ✅ **Parser LL(1)** - Análise sintática descendente preditiva
- ✅ **Parser SLR(1)** - Análise sintática ascendente com autômato LR(0)
- ✅ **Gramática Completa** - Suporta declarações, expressões, condicionais e loops
- ✅ **Cálculo FIRST/FOLLOW** - Automático para análise sintática
- ✅ **Log Detalhado** - Trace completo salvo em arquivo

## 🚀 Como Rodar

### Requisitos
- Python 3.7+

### Execução
```bash
python compilador.ipynb
```

O programa irá:
1. Analisar o código-fonte de exemplo
2. Executar análise léxica
3. Executar parser LL(1)
4. Executar parser SLR(1)
5. Salvar trace completo em `output_compilador_completo.txt`

## 📝 Linguagem Suportada
```c
main() {
    int x;
    float y;
    x = 10;
    y = 3.14;
    
    if (x < 20) {
        x = x + 1;
    } else {
        x = x - 1;
    }
    
    while (x > 0) {
        x = x - 1;
    }
}
```

## 📊 Resultados
```
✓ Análise Léxica:  SUCESSO
✓ Parser LL(1):    ACEITO
✓ Parser SLR(1):   ACEITO
```

## 📂 Estrutura
```
compilador.ipynb          # Notebook principal com todas as células
output_compilador_completo.txt  # Log detalhado (gerado automaticamente)
```

## 🎓 Características Técnicas

- **Tokens**: 40+ tipos (palavras-chave, operadores, identificadores)
- **Gramática**: 40+ produções transformadas para LL(1)
- **Estados LR(0)**: 91 estados no autômato SLR
- **Tabela LL(1)**: Sem conflitos
- **Tabela SLR(1)**: Sem conflitos shift-reduce ou reduce-reduce

## 📖 Documentação

O código está dividido em 8 células no Jupyter Notebook:
1. Importações
2. Analisador Léxico
3. Gramática LL(1)
4. Cálculo FIRST/FOLLOW
5. Parser LL(1)
6. Parser SLR(1)
7. Funções de Demonstração
8. Execução Principal

---

**Desenvolvido para disciplina de Compiladores** 🎯
```

---
