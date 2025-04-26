# ee451-assignment-6a-solved
**TO GET THIS SOLUTION VISIT:** [EE451 Assignment 6a Solved](https://www.ankitcodinghub.com/product/ee451-assignment-6a-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;100479&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EE451 Assignment 6a Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
1. Examples

Copy example files to your home directory.

1. Login to HPC 2. Copy

cp -r /project/xuehaiqi_652/6a .

The hello.cu contains the CUDA implementation of HelloWorld.

<ol>
<li>Login to HPC</li>
<li>Setup MPI toolchain:</li>
<li>Compilenvcc -O3 hello.cu</li>
<li>RunThe option -t specifies the limit of run time. Setting it as a small number will get your program scheduled earlier. For more information on srun options, you can use man srun to find out.</li>
<li>Profile (optional)srun -n1 –gres=gpu:p100:1 –partition=debug nvprof ./a.out</li>
<li>Allocate a machine</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
module purge

module load gcc /8.3.0 cuda /10.1.243

</div>
</div>
<div class="layoutArea">
<div class="column">
srun -n1 –gres=gpu:1 -t1 ./a.out

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
salloc -n1 –gres=gpu:1 –mem=16G -t10

// After the allocation, you will log on the machine and have 10 minutes to perform multiple operations

./a.out

// edit , compile , and run again without waiting for a new allocation

./a.out ./a.out

</div>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
<ol start="2">
<li>(15 points) Refer to the file globalVaribale.cu. Declare statically a global float array with a size of five elements. Initialize the global array with the same value of 3.14. Modify the kernel to let each thread change the value of the array element with the same index as the thread index. Let the value be multiplied with the thread index. Invoke the kernel with five threads.</li>
<li>(15 points) Modify sumArrayZerocpy.cu to access A, B, and C at an offset. Compare performance with and without L1 cache enabled.</li>
<li>(15 points) Modify readWriteSegment.cu. Apply an unrolling factor of four to readWriteOffset and compare performance with the original.</li>
<li>(15 points) Modify transpose.cu. Refer to the kernel transposeUnroll4Row. Imple- ment a new kernel, transposeUnroll8Row, to let each thread handle eight elements. Compare the performance with existing kernels.</li>
<li>(15 points) Modify transpose.cu. Refer to the kernels transposeDiagonalCol and transposeUnroll4Row. Implement a new kernel, transposeDiagonalColUnroll4, to let each thread handle four elements. Compare the performance with existing kernels.</li>
<li>(25 points) A CUDA program has 2K threads. 3 GB of data need to be transferred from CPU to GPU and 1 GB of result data need to be transferred back from GPU to CPU. Data transfer is through PCIe whose bandwidth is 16 GB/s. The GPU has 1K CUDA cores and can run at most 1K threads in parallel. Each CUDA core runs at 1 GHz and is able to perform 1 multiply-add operation in each clock cycle. Each access to global memory takes 100 cycles. Assume each thread needs 10 memory accesses to the global memory and 100 multiply-add operations. What is the execution time of the CUDA program in the best case? Clearly state your assumptions.The total execution time consists of three parts: Data transfer latency (CPU to GPU), Kernel execution and Data transfer latency (GPU to CPU).</li>
</ol>
</div>
</div>
</div>
