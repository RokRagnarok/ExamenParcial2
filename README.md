# ExamenParcial2
## Gustavo Zumaya Miranda

# SimpleMathAoS
CUDA memcpy DtoH: Esta actividad representa el 80.19% del tiempo de la GPU con un tiempo medio de ejecución de 11.652 milisegundos
implica 2 llamadas para transferir datos desde el dispositivo GPU al host (CPU)Los tiempos de ejecución mínimo y máximo para una llamada individual son 8,6804 milisegundos y 14.623 milisegundos respectivamente.
CUDA memcpy HtoD: esta actividad representa el 18,05% del tiempo de la GPU, y una sola llamada tarda 5,2457 milisegundos esta es una operación de transferencia de memoria desde el host (CPU) al dispositivo GPU.
warmup: (innerStruct, InnerStruct, int) **: esta función representa el 0,88% del tiempo de la GPU y tiene un tiempo de ejecución de 256,10 microsegundos.Se llama una vez y parece ser una función relacionada con el trabajo de la GPU.
testInnerStruct(innerStruct, InnerStruct, int)**: esta función también representa el 0.88% del tiempo de la GPU y tiene un tiempo de ejecución de 255.85 microsegundos.Similar a la función anterior está relacionada con el trabajo de la GPU.
cudaMalloc: esta llamada API representa el 88,83% del tiempo de llamada API, con un total de 566,38 milisegundos y se utiliza para asignar memoria en la GPU Esta llamada se hizo dos veces.
cudaDeviceReset: esta llamada API representa el 5,61% del tiempo de llamada API, con un tiempo de ejecución de 35,742 milisegundos,se llama una vez y se utiliza para restablecer el dispositivo GPU.
cudaMemcpy: esta llamada API representa el 4,90% del tiempo de llamada API, con un tiempo de ejecución promedio de 10,422 milisegundos. Se llamó tres veces y se utiliza para copiar datos entre el host y la GPU.
cuDeviceGetPCIBusId: esta llamada API representa el 0,34% del tiempo de llamada API, con un tiempo de ejecución de 2,1562 milisegundos. Fue llamado una vez.
cudaFree: esta llamada API representa el 0,19% del tiempo de llamada API y tiene un tiempo de ejecución promedio de 610,00 microsegundos. Se llamó dos veces y se utiliza para liberar memoria en la GPU.
cudaDeviceSynchronize: esta llamada API representa el 0,11% del tiempo de llamada API, con un tiempo de ejecución promedio de 334,95 microsegundos. Se llamó dos veces y se utiliza para sincronizar el dispositivo GPU.
cudaLaunchKernel: esta llamada API representa el 0,03% del tiempo de llamada API, con un tiempo de ejecución promedio de 80,800 microsegundos. Se llamó dos veces y se utiliza para iniciar núcleos de GPU.
# SimpleMathSoA
CUDA memcpy DtoH: Esta actividad representa el 73,35% del tiempo de la GPU, con un tiempo total de ejecución de 12,215 milisegundos.Implica 2 llamadas para copiar datos desde el dispositivo GPU al host (CPU).El tiempo medio de ejecución de cada llamada es de 6,1076 milisegundos, con un mínimo de 3,7599 milisegundos y un máximo de 8,4554 milisegundos.
CUDA memcpy HtoD: esta actividad representa el 23,58% del tiempo de la GPU, y una sola llamada tarda 3,9265 milisegundos. Representa una operación de transferencia de memoria desde el host (CPU) al dispositivo GPU.
Warmup2(InnerArray, InnerArray, int)**: Esta función representa el 1,54% del tiempo de la GPU y tiene un tiempo de ejecución de 256,42 microsegundos. Se llamó una vez y parece estar relacionado con el trabajo de la GPU.
testInnerArray(InnerArray, InnerArray, int)**: esta función también representa el 1,54% del tiempo de la GPU y tiene un tiempo de ejecución de 256,03 microsegundos. Al igual que la función anterior, parece estar relacionada con el trabajo de la GPU.
cudaMalloc: esta llamada API representa el 90,98% del tiempo de llamada API, con un tiempo total de ejecución de 584,89 milisegundos. Se utiliza para asignar memoria en la GPU y se llamó dos veces.
cudaDeviceReset: esta llamada API representa el 5,47% del tiempo de llamada API, con un tiempo de ejecución de 35,165 milisegundos. Se llama una vez y se utiliza para restablecer el dispositivo GPU.
cudaMemcpy: esta llamada API representa el 2,89% del tiempo de llamada API, con un tiempo de ejecución promedio de 6,1881 milisegundos. Se llamó tres veces y se utiliza para copiar datos entre el host y la GPU.
cuDeviceGetPCIBusId: esta llamada API representa el 0,39% del tiempo de llamada API, con un tiempo de ejecución de 2,4897 milisegundos. Fue llamado una vez.
cudaFree: esta llamada API representa el 0,15% del tiempo de llamada API y tiene un tiempo de ejecución promedio de 981,80 microsegundos. Se llamó dos veces y se utiliza para liberar memoria en la GPU.
cudaDeviceSynchronize: esta llamada API representa el 0.11% del tiempo de llamada API con un tiempo de ejecución promedio de 682.20 microsegundos se llamó dos veces y se utiliza para sincronizar el dispositivo GPU.
cudaLaunchKernel: esta llamada API representa el 0.01% del tiempo de llamada API con un tiempo de ejecución promedio de 94.200 microsegundos se llamó dos veces y se utiliza para iniciar núcleos de GPU.
# sumArrayZerocpy
sumArraysZeroCopy(float, float, float*, int)**: esta actividad representa el 33,33% del tiempo de la GPU, con un tiempo de ejecución de 3,5200 microsegundos. Representa la ejecución de una función que funciona con matrices de GPU.
CUDA memcpy DtoH: esta actividad representa el 22,73% del tiempo de la GPU, con dos llamadas para copiar datos del dispositivo GPU al host (CPU). El tiempo medio de ejecución de cada llamada es de 1,2000 microsegundos, con un mínimo de 1,1840 microsegundos y un máximo de 1,2160 microsegundos.
sumArrays(float, float, float*, int)**: esta actividad representa el 22,12% del tiempo de la GPU, con un tiempo de ejecución de 2,3360 microsegundos. Representa la ejecución de otra función que funciona con matrices de GPU.
CUDA memcpy HtoD: esta actividad representa el 21,82% del tiempo de la GPU, con dos llamadas para copiar datos desde el host (CPU) al dispositivo GPU. El tiempo medio de ejecución de cada llamada es de 1,1520 microsegundos, con un mínimo de 864 nanosegundos y un máximo de 1,4400 microsegundos.

cudaMalloc: esta llamada API representa el 94,24% del tiempo de llamada API, con un tiempo total de ejecución de 583,14 milisegundos. Se utiliza para asignar memoria en la GPU y se llamó tres veces.
cudaDeviceReset: esta llamada API representa el 5,09% del tiempo de llamada API, con un tiempo de ejecución de 31,475 milisegundos. Se llama una vez y se utiliza para restablecer el dispositivo GPU.
cuDeviceGetPCIBusId: esta llamada API representa el 0,35% del tiempo de llamada API, con un tiempo de ejecución de 2,1756 milisegundos. Se llamó una vez y se utiliza para recuperar el ID del bus PCI de la GPU.
cudaHostAlloc: esta llamada API representa el 0,16% del tiempo de llamada API, con un tiempo total de ejecución de 988,60 microsegundos. Se llamó dos veces y se utiliza para asignar memoria a la que pueden acceder tanto el host como la GPU.
cudaFreeHost: esta llamada API representa el 0,06% del tiempo de llamada API, con un tiempo total de ejecución de 368,90 microsegundos. Se llamó dos veces y se usa para liberar memoria asignada con cudaHostAlloc.
cudaMemcpy: esta llamada a la API representa el 0,06% del tiempo de llamada a la API, con cuatro llamadas para copiar datos entre el host y la GPU. El tiempo medio de ejecución de cada llamada es de 89.500 microsegundos.
# sumMatrixGPUManaget
sumMatrixGPU(float, float, float*, int, int)**: Esta función representa el 100,00% del tiempo de la GPU, con un tiempo total de ejecución de 12,948 milisegundos. Implica dos llamadas y tiene un tiempo de ejecución promedio de 6,4741 milisegundos. El tiempo mínimo de ejecución para una sola llamada es de 288,67 microsegundos, mientras que el máximo es de 12,660 milisegundos. Esta función parece ser la carga de trabajo principal de la GPU.
​cudaMallocManaged: esta llamada API representa el 91,39% del tiempo de llamada API, con un tiempo total de ejecución de 815,38 milisegundos. Se utiliza para asignar memoria administrada en la GPU y se llamó cuatro veces.
cudaDeviceReset: esta llamada API representa el 3,45% del tiempo de llamada API, con un tiempo de ejecución de 30,801 milisegundos. Se llama una vez y se utiliza para restablecer el dispositivo GPU.
cudaFree: esta llamada API representa el 3,31% del tiempo de llamada API, con un tiempo total de ejecución de 29,569 milisegundos. Fue llamado cuatro veces y sirve para liberar memoria de la GPU.
cudaDeviceSynchronize: esta llamada API representa el 1,52% del tiempo de llamada API, con un tiempo de ejecución de 13,583 milisegundos. Se llama una vez y se utiliza para sincronizar el dispositivo GPU.
cuDeviceGetPCIBusId: esta llamada API representa el 0,24% del tiempo de llamada API, con un tiempo de ejecución de 2,1681 milisegundos. Se llamó una vez y se utiliza para recuperar el ID del bus PCI de la GPU.
cudaLaunchKernel: esta llamada API representa el 0,07% del tiempo de llamada API, con un tiempo total de ejecución de 644,20 microsegundos. Se llamó dos veces y se utiliza para iniciar núcleos de GPU.
# sumMatrixGPUManual
CUDA memcpy HtoD: esta actividad representa el 65,52% del tiempo de la GPU, con dos llamadas para copiar datos desde el host (CPU) al dispositivo GPU. El tiempo medio de ejecución de cada llamada es de 13.550 milisegundos, con un mínimo de 8.3698 milisegundos y un máximo de 18.731 milisegundos.
CUDA memcpy DtoH: esta actividad representa el 30,63% del tiempo de la GPU, y una sola llamada tarda 12,669 milisegundos. Representa una operación de transferencia de memoria desde el dispositivo GPU al host (CPU).
sumMatrixGPU(float, float, float*, int, int)**: esta función representa el 2,69% del tiempo de la GPU y tiene un tiempo de ejecución de 1,1118 milisegundos. Se llamó dos veces y es parte de la carga de trabajo de la GPU.
CUDA memset: esta actividad representa el 1,16% del tiempo de la GPU, con dos llamadas para configurar la memoria de la GPU en un valor específico. El tiempo medio de ejecución de cada llamada es de 239,71 microsegundos.
# transpose
CUDA memcpy HtoD: esta actividad representa el 86,82% del tiempo de la GPU, y una sola llamada tarda 1,9853 milisegundos. Representa la transferencia de datos desde el host (CPU) al dispositivo GPU.
copyRow(float, float, int, int)**: esta función representa el 6,62% del tiempo de la GPU, con un tiempo de ejecución de 151,49 microsegundos. Se llamó una vez y es parte de la carga de trabajo de la GPU.
calentamiento (float, float, int, int) **: esta función representa el 6,56% del tiempo de la GPU, con un tiempo de ejecución de 150,02 microsegundos. Se llamó una vez y es parte de la carga de trabajo de la GPU.
cudaMalloc: esta llamada API representa el 86,44% del tiempo de llamada API, con un tiempo total de ejecución de 634,10 milisegundos. Se llamó dos veces y se utiliza para asignar memoria en la GPU.
cudaDeviceReset: esta llamada API representa el 12,79% del tiempo de llamada API, con un tiempo de ejecución de 93,791 milisegundos. Se llama una vez y se utiliza para restablecer el dispositivo GPU.
cudaMemcpy: esta llamada API representa el 0,32% del tiempo de llamada API, con un tiempo de ejecución de 2,3634 milisegundos. Se utiliza para copiar datos entre el host y la GPU.
cuDeviceGetPCIBusId: esta llamada API representa el 0,31% del tiempo de llamada API, con un tiempo de ejecución de 2,2569 milisegundos. Se llama una vez y se utiliza para recuperar el ID del bus PCI de la GPU.
cudaFree: esta llamada a la API representa el 0,07% del tiempo de llamada a la API, con dos llamadas para liberar memoria de la GPU.
cudaDeviceSynchronize: esta llamada API representa el 0,06% del tiempo de llamada API, con dos llamadas para sincronizar el dispositivo GPU.
cudaLaunchKernel: esta llamada a la API representa el 0,01 % del tiempo de llamada a la API, con dos llamadas para iniciar núcleos de GPU.
# writeSegment
CUDA memcpy DtoH: esta actividad representa el 65,98% del tiempo de la GPU, con tres llamadas que tardan un promedio de 704,29 microsegundos cada una. Representa la transferencia de datos desde la GPU al host (CPU).
CUDA memcpy HtoD: esta actividad representa el 29,36% del tiempo de la GPU, con dos llamadas que tardan un promedio de 470,12 microsegundos cada una. Representa la transferencia de datos desde el host (CPU) a la GPU.
writeOffset(float, float, float*, int, int)**: esta función representa el 1,55% del tiempo de la GPU, con un tiempo de ejecución de 49,504 microsegundos. Se llamó una vez y es parte de la carga de trabajo de la GPU.
calentamiento (float, float, float*, int, int) **: esta función representa el 1,49% del tiempo de la GPU, con un tiempo de ejecución de 47,712 microsegundos. Se llamó una vez y es parte de la carga de trabajo de la GPU.
writeOffsetUnroll2(float, float, float*, int, int)**: esta función representa el 0,91% del tiempo de la GPU, con un tiempo de ejecución de 29,120 microsegundos. Se llamó una vez y es parte de la carga de trabajo de la GPU.
writeOffsetUnroll4(float, float, float*, int, int)**: esta función representa el 0,72% del tiempo de la GPU, con un tiempo de ejecución de 23,072 microsegundos. Se llamó una vez y es parte de la carga de trabajo de la GPU.
cudaMalloc: This API call accounts for 92.61% of the API call time, with a total execution time of 579.23 milliseconds. It was called three times and is used to allocate memory on the GPU.
cudaDeviceReset: This API call accounts for 6.01% of the API call time, with an execution time of 37.576 milliseconds. It is called once and is used to reset the GPU device.
cudaMemcpy: This API call accounts for 0.83% of the API call time, with a total execution time of 5.1802 milliseconds. It is used for copying data between the host and GPU.
cuDeviceGetPCIBusId: This API call accounts for 0.34% of the API call time, with an execution time of 2.1550 milliseconds. It is called once and is used to retrieve the PCI bus ID of the GPU.
cudaFree: This API call accounts for 0.11% of the API call time, with three calls to free GPU memory.
cudaDeviceSynchronize: This API call accounts for 0.06% of the API call time, with four calls to synchronize the GPU device.
cudaLaunchKernel: This API call accounts for 0.04% of the API call time, with four calls for launching GPU kernels.
# memTransfer
CUDA memcpy HtoD: Esta actividad representa el 52,15% del tiempo de la GPU, con un tiempo total de 2,1117 milisegundos. Representa la transferencia de datos desde el host (CPU) a la GPU.
CUDA memcpy DtoH: Esta actividad representa el 47,85% del tiempo de la GPU, con un tiempo total de 1,9374 milisegundos. Representa la transferencia de datos desde la GPU al host (CPU).
cudaMalloc: This API call accounts for 93.74% of the API call time, with a total execution time of 577.35 milliseconds. It is called once and is used for allocating memory on the GPU.
cudaDeviceReset: This API call accounts for 5.15% of the API call time, with a total execution time of 31.729 milliseconds. It is called once and is used to reset the GPU device.
cudaMemcpy: This API call accounts for 0.71% of the API call time, with two calls to copy data between the host and GPU.
cuDeviceGetPCIBusId: This API call accounts for 0.34% of the API call time, with a total execution time of 2.0994 milliseconds. It is called once and is used to retrieve the PCI bus ID of the GPU.
cudaFree: This API call accounts for 0.05% of the API call time, with a single call to free GPU memory.
# pinMemTransfer
CUDA memcpy HtoD: esta actividad representa la transferencia de datos desde la memoria del host (CPU) a la memoria del dispositivo (GPU). Esta operación es la más cara en términos de tiempo, representando el 50,57% del tiempo de la GPU con una duración de 1,3036 milisegundos. Se realiza una única llamada y el tiempo medio es de 1,3036 milisegundos.
CUDA memcpy DtoH: esta actividad representa la transferencia de datos desde la memoria del dispositivo (GPU) a la memoria del host (CPU). Es una operación similar en el tiempo a la anterior, ya que representa el 49,43% del tiempo de la GPU con una duración de 1,2743 milisegundos. También se realiza una única llamada y el tiempo medio es de 1,2743 milisegundos.
​cudaHostAlloc: esta llamada API representa el 93,65% del tiempo total de la llamada API con una duración de 564,84 milisegundos. Se realiza una única llamada y se utiliza para asignar memoria en el host (CPU) para que sea accesible desde el dispositivo (GPU).
cudaDeviceReset: esta llamada API representa el 5,15% del tiempo total de la llamada API con una duración de 31.051 milisegundos. Se utiliza para restablecer el dispositivo GPU a su estado inicial.
cudaMemcpy: esta llamada a la API representa el 0,45% del tiempo total de la llamada a la API con dos llamadas. Se utiliza para copiar datos entre el host y el dispositivo.
cuDeviceGetPCIBusId: esta llamada a la API representa el 0,34 % del tiempo total de la llamada a la API con una duración de 2,0604 milisegundos. Se realiza una única llamada y se utiliza para obtener el ID del bus PCI del dispositivo GPU.
cudaFreeHost: esta llamada API representa el 0,30% del tiempo total de la llamada API con una duración de 1,8091 milisegundos. Se realiza una única llamada y se utiliza para liberar memoria asignada en el host.
cudaMalloc: esta llamada API representa el 0,06% del tiempo total de la llamada API con una duración de 342,90 microsegundos. Se realiza una única llamada y se utiliza para asignar memoria en el dispositivo GPU.
cudaFree: esta llamada API representa el 0,04% del tiempo total de la llamada API con una duración de 261,00 microsegundos. Se realiza una única llamada y se utiliza para liberar la memoria asignada en el dispositivo GPU.
# readSegment
CUDA memcpy DtoH: esta operación ocupa el 49,71% del tiempo e implica copiar datos del dispositivo (GPU) al host (CPU).
CUDA memcpy HtoD: esta operación ocupa el 45,41% del tiempo e implica copiar datos desde el host (CPU) al dispositivo (GPU).
readOffset(float*, float*, float*, int, int): esta es una función de GPU personalizada que ocupa el 2,48% del tiempo.
calentamiento (float*, float*, float*, int, int): otra función de GPU personalizada, que ocupa el 2,40% del tiempo.
cudaMalloc: esta es la llamada API que consume más tiempo y representa el 93,88% del tiempo. Se utiliza para asignar memoria en la GPU.
cudaDeviceReset: esto ocupa el 5,02% del tiempo y se utiliza para restablecer el dispositivo GPU.
cudaMemcpy: ocupa el 0,52% del tiempo y se utiliza para copiar datos entre el host y el dispositivo.
cuDeviceGetPCIBusId: esta llamada API ocupa el 0,40 % del tiempo y se utiliza para recuperar el ID del bus PCI del dispositivo.
cudaFree: esta llamada API ocupa el 0,13% del tiempo y se utiliza para liberar memoria asignada en la GPU.
cudaDeviceSynchronize: esta llamada ocupa el 0,03% del tiempo y se utiliza para sincronizar el dispositivo GPU.
cudaLaunchKernel: ocupa el 0,01% del tiempo y se utiliza para iniciar núcleos de GPU.
cuDeviceGetAttribute: esta llamada API representa el 0,00 % del tiempo y se utiliza para recuperar atributos del dispositivo.
cudaSetDevice: esta llamada API ocupa el 0,00% del tiempo y se utiliza para configurar el dispositivo CUDA actual.
cudaGetDeviceProperties: esta llamada ocupa el 0,00% del tiempo y se utiliza para recuperar propiedades del dispositivo CUDA actual.
cudaGetLastError: esta llamada a la API ocupa el 0,00 % del tiempo y se utiliza para comprobar el último error de CUDA.
cuDeviceGetCount: esta llamada API ocupa el 0,00% del tiempo y se utiliza para recuperar la cantidad de dispositivos CUDA.
cuDeviceGet: esta llamada API ocupa el 0,00% del tiempo y se utiliza para recuperar un dispositivo CUDA por ordinal.
cuDeviceGetName: esta llamada API ocupa el 0,00% del tiempo y se utiliza para recuperar el nombre de un dispositivo CUDA.
cuDeviceTotalMem: esta llamada API ocupa el 0,00% del tiempo y se utiliza para recuperar la memoria total de un dispositivo CUDA.
cuDeviceGetUuid: esta llamada API ocupa el 0,00% del tiempo y se utiliza para recuperar el UUID de un dispositivo CUDA.
# readSegmentUnroll
CUDA memcpy DtoH: esta operación ocupa el 64,13% del tiempo e implica copiar datos del dispositivo (GPU) al host (CPU).
CUDA memcpy HtoD: esta operación ocupa el 27,79% del tiempo e implica copiar datos desde el host (CPU) al dispositivo (GPU).
CUDA memset: esta operación ocupa el 1,94% del tiempo y se utiliza para establecer una región de memoria en la GPU en un valor específico.
readOffsetUnroll4(float*, float*, float*, int, int): esta es una función de GPU personalizada que ocupa el 1,56% del tiempo.
readOffset(float*, float*, float*, int, int): otra función de GPU personalizada, que ocupa el 1,55% del tiempo.
readOffsetUnroll2(float*, float*, float*, int, int): otra función de GPU personalizada, que ocupa el 1,54% del tiempo.
warmup (float*, float*, float*, int, int): otra función de GPU personalizada más, que ocupa el 1,49% del tiempo.
cudaMalloc: esta es la llamada API que consume más tiempo y representa el 93,30% del tiempo. Se utiliza para asignar memoria en la GPU.
cudaDeviceReset: esto ocupa el 5,46% del tiempo y se utiliza para restablecer el dispositivo GPU.
cudaMemcpy: ocupa el 0,69% del tiempo y se utiliza para copiar datos entre el host y el dispositivo.
cuDeviceGetPCIBusId: esta llamada API ocupa el 0,32% del tiempo y se utiliza para recuperar el ID del bus PCI del dispositivo.
cudaFree: esta llamada API ocupa el 0,12% del tiempo y se utiliza para liberar memoria asignada en la GPU.
cudaDeviceSynchronize: esta llamada ocupa el 0,06% del tiempo y se utiliza para sincronizar el dispositivo GPU.
cudaMemset: esta llamada API ocupa el 0,02% del tiempo y se utiliza para establecer una región de la memoria de la GPU en un valor específico.
cudaLaunchKernel: ocupa el 0,01% del tiempo y se utiliza para iniciar núcleos de GPU.
cuDeviceGetAttribute: esta llamada API representa el 0,00 % del tiempo y se utiliza para recuperar atributos del dispositivo.
cudaGetDeviceProperties: esta llamada ocupa el 0,00% del tiempo y se utiliza para recuperar propiedades del dispositivo CUDA actual.
cudaSetDevice: esta llamada API ocupa el 0,00% del tiempo y se utiliza para configurar el dispositivo CUDA actual.
cudaGetLastError: esta llamada a la API ocupa el 0,00 % del tiempo y se utiliza para comprobar el último error de CUDA.
cuDeviceGet: esta llamada API ocupa el 0,00% del tiempo y se utiliza para recuperar un dispositivo CUDA por ordinal.
cuDeviceGetCount: esta llamada API ocupa el 0,00% del tiempo y se utiliza para recuperar la cantidad de dispositivos CUDA.
cuDeviceGetName: esta llamada API ocupa el 0,00% del tiempo y se utiliza para recuperar el nombre de un dispositivo CUDA.
cuDeviceTotalMem: esta llamada API ocupa el 0,00% del tiempo y se utiliza para recuperar la memoria total de un dispositivo CUDA.
cuDeviceGetUuid: esta llamada API ocupa el 0,00% del tiempo y se utiliza para recuperar el UUID de un dispositivo CUDA.
