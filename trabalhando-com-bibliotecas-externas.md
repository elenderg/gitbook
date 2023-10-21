# Trabalhando com Bibliotecas externas

Para utilizar bibliotecas externas, basta utilizar a palavra-chave <mark style="color:blue;">`Processe`</mark>, seguido do nome da biblioteca (entre aspas duplas), juntamente com o nome da função (case-sensitive, entre aspas duplas). Caso seja necessário repassar argumentos para a função,  Exemplos:

<mark style="color:blue;">`Processe`</mark>` ``"user32.dll" "CloseClipboard".`



Caso seja necessário repassar argumentos para a função, _utilize a palavra-chave_ _<mark style="color:green;">`com`</mark>_.

<mark style="color:blue;">`Processe`</mark>`"user32.dll" "OpenClipboard"`<mark style="color:green;">`com`</mark>`a janela principal do programa.`



Para obter o valor de retorno da função que foi invocada, _utilize a palavra-chave_ _<mark style="color:purple;">`retornando`</mark>_.

<mark style="color:blue;">`Processe`</mark>`"user32.dll" "GetClipboardData"`<mark style="color:green;">`com`</mark>`o formato de texto`_<mark style="color:purple;">`retornando`</mark>_`um número identificador.`
