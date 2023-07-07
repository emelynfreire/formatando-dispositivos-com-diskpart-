# formatando-dispositivos-com-diskpart-

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
![image](https://github.com/emelynfreire/formatando-dispositivos-com-diskpart-/assets/18231484/182b06e8-5975-4744-a64a-7cbe58e55524)




