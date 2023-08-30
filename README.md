# ph
foi feito um projeto em aula
    elif opcao == 4:
        aluno_media = input('Digite o nome do aluno: ')
        if aluno_media in alunos:
            media = sum(alunos[aluno_media]) / len(alunos[aluno_media])
            print(f'A média do(a) {aluno_media} é {media:.2f}')
        else:
            print('Aluno não encontrado.')

    elif opcao == 5:
        rank = sorted(alunos.keys(), key=lambda aluno: sum(alunos[aluno]), reverse=True)
        print('Rank dos Alunos:')
        for i, aluno in enumerate(rank, start=1):
            media = sum(alunos[aluno]) / len(alunos[aluno])
            print(f'{i}. {aluno}: Média {media:.2f}')

    elif opcao == 6:
        for aluno, notas in alunos.items():
            media = sum(notas) / len(notas)
            print(f'{aluno}: Notas {notas}, Média {media:.2f}')

    elif opcao == 7:
        print('Encerrando o programa...')

    else:
        print('Opção inválida. Por favor, escolha uma opção válida.')

print('Muito obrigado')
