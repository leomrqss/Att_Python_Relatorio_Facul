# Att_Python_Relat-rio_Facul
Sistema de Gestão de Notas de Alunos

# Sistema de Gestão de Notas de Alunos

# Lista de notas simulada (troque os valores para testar)
notas_aluno = [8.0, 7.5, 7.0]

# Função para calcular a média
def calcular_media(notas):
    if len(notas) == 0:
        return 0
    return sum(notas) / len(notas)

# Função para determinar a situação
def verificar_situacao(media):
  #Verifica a situação do aluno com base na média.
    #- Se média >= 7 → Aprovado
    #- Se média < 7  → Reprovado
    if media >= 7:
        return "Aprovado"
    else:
        return "Reprovado"

# Função para exibir o relatório final
def exibir_relatorio(notas, media, situacao):
  #Exibe as notas, a média calculada e a situação final do aluno.
    print("\nRELATÓRIO FINAL")
    print(f"Notas: {notas}")
    print(f"Média: {media:.2f}")
    print(f"Situação: {situacao}")

# Programa principal

#Calcula a média do aluno
media_aluno = calcular_media(notas_aluno)
# Determina a situação (aprovado ou reprovado)
situacao_aluno = verificar_situacao(media_aluno)
# Mostra o relatório final
exibir_relatorio(notas_aluno, media_aluno, situacao_aluno)
