Formatando dispositivos corrompidos no Windows usando o Diskpart

Problema: Ao inserir meu pendrive no notebook, ele não estava sendo reconhecido e solicitava formatação, mas não era possível formatá-lo normalmente.

Solução:

    Abra o prompt de comando (CMD) e digite "diskpart".

    Após abrir o diskpart, liste os discos e partições detectados pelo dispositivo usando o comando:
    
No CMD DIGITAR "diskpart":
Logo após abrir o diskpart você poderá listar os discos e partições visualizadas pelo dispositivo:
DISKPART> list disk
![image](https://github.com/emelynfreire/formatando-dispositivos-com-diskpart-/assets/18231484/70814a7d-7a9f-417e-9130-2b1f18c989ae)

Selecione o disco que pretende formatar pelo comando: 
DISKPART> select disk 4
DISKPART> clean
DISKPART> create partition primary

![image](https://github.com/emelynfreire/formatando-dispositivos-com-diskpart-/assets/18231484/e5ec8e5c-8638-47d2-8c1f-ce140345474e)

Caso de algum erro, repita o processo:
![image](https://github.com/emelynfreire/formatando-dispositivos-com-diskpart-/assets/18231484/30c8abef-394d-4332-9cd6-88e72feed884)

Quando retorno:
DiskPart criou com êxito a partição especificada.

Você escolherá o formato de partição a ser formatado:
DISKPART> format fs= ntfs quick

Obs: ntfs é o tipo de partição.
quick refere-se a formatação rápidam você tem a opção se fazer a formatação completa mas demorará mais. Se caso a rápida não resolver seu problema tente a completa:
DISKPART> format fs= ntfs

![image](https://github.com/emelynfreire/formatando-dispositivos-com-diskpart-/assets/18231484/182b06e8-5975-4744-a64a-7cbe58e55524)

Em este computador podemos ver que o pendrive foi formatado e está funcionando perfeitamente.
![image](https://github.com/emelynfreire/formatando-dispositivos-com-diskpart-/assets/18231484/d264d636-c29b-42f4-9898-795c663cbfb2)

Sequência de comandos:

![image](https://github.com/emelynfreire/formatando-dispositivos-com-diskpart-/assets/18231484/797ff8bd-cb38-4738-81f7-7dfb8e90c751)






