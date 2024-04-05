<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">CfdOF：FreeCAD 的计算流体动力学 (CFD) 工作台</font></font></h1><a id="user-content-cfdof-a-computational-fluid-dynamics-cfd-workbench-for-freecad" class="anchor" aria-label="永久链接：CfdOF：FreeCAD 的计算流体动力学 (CFD) 工作台" href="#cfdof-a-computational-fluid-dynamics-cfd-workbench-for-freecad"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"></font><a href="https://freecadweb.org" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该工作台旨在帮助用户在FreeCAD</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">建模器中设置和运行 CFD 分析，并用作流行的 OpenFOAM® CFD 工具包（ </font></font><a href="http://www.openfoam.org" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">www.openfoam.org</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="http://www.openfoam.com" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">www.openfoam.com</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> ）
的前端 (GUI) </font><font style="vertical-align: inherit;">。它指导用户在运行模拟之前选择相关物理场、指定材料属性、生成网格、分配边界条件以及选择解算器设置。指定最佳实践以最大限度地提高求解器的稳定性。</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/jaheyns/CfdOF/blob/master/Doc/Resources/boiler.png"><img src="/jaheyns/CfdOF/raw/master/Doc/Resources/boiler.png" alt="截屏" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">免责声明：本产品未经 OpenCFD Limited（OpenFOAM 软件的生产商和分销商（通过
</font></font><a href="http://www.openfoam.com" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">www.openfoam.com</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）以及 OPENFOAM® 和 OpenCFD® 商标的所有者）批准或认可</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">特征</font></font></h2><a id="user-content-features" class="anchor" aria-label="永久链接：特点" href="#features"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">当前的：</font></font></h3><a id="user-content-current" class="anchor" aria-label="永久链接： 当前：" href="#current"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">流动物理学</font></font></h4><a id="user-content-flow-physics" class="anchor" aria-label="永久链接：流动物理学" href="#flow-physics"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不可压缩的层流（simpleFoam、pimpleFoam）</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">支持各种 RANS、LES 和 DES 湍流模型</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不可压缩自由表面流（interFoam、多相InterFoam）</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可压缩浮力流（buoyantSimpleFoam、buoyantPimpleFoam）</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">高速可压缩流 ( </font></font><a href="https://hisa.gitlab.io" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">HiSA</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> )</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">多孔区域和多孔挡板</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">基础材料数据库</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用潜在求解器进行流初始化</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">任意无源标量传输函数的解</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">网格划分</font></font></h4><a id="user-content-meshing" class="anchor" aria-label="永久链接：网格划分" href="#meshing"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">带边界层的切割单元笛卡尔网格划分 (cfMesh)</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">带挡板的切割单元笛卡尔网格划分 (snappyHexMesh)</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 Gmsh 进行四面体网格划分，包括转换为多面体双网格</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">网格划分后检查网格</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">支持支持求解器的动态网格自适应</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">后处理和监控</font></font></h4><a id="user-content-post-processing-and-monitoring" class="anchor" aria-label="永久链接：后处理和监控" href="#post-processing-and-monitoring"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 Paraview 进行后处理</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对基于力的函数对象（力、力系数）的基本支持</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对探针的基本支持</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">其他特性</font></font></h4><a id="user-content-other-features" class="anchor" aria-label="永久链接：其他功能" href="#other-features"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在 Windows 7-11 和 Linux 上运行</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">单元/回归测试</font></font></li>
<li>Case builder using an extensible template structure</li>
<li>Macro scripting</li>
<li>Support for distributed parallel (cluster) runs via mpiexec &amp; --hostfile</li>
</ul>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Platforms supported</h3><a id="user-content-platforms-supported" class="anchor" aria-label="永久链接：支持的平台" href="#platforms-supported"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Linux</h4><a id="user-content-linux" class="anchor" aria-label="永久链接：Linux" href="#linux"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Any system on which FreeCAD and the prerequisites listed below can be installed.</p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Windows</h4><a id="user-content-windows" class="anchor" aria-label="永久链接：Windows" href="#windows"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Windows 7-11; 64-bit version is required.</p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">macOS</h4><a id="user-content-macos" class="anchor" aria-label="永久链接：macOS" href="#macos"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Not widely tested, but success has been reported. See
<a href="https://forum.freecadweb.org/viewtopic.php?f=37&amp;t=63782&amp;p=547611#p547578" rel="nofollow">the following forum post</a>
for instructions.</p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Getting started</h2><a id="user-content-getting-started" class="anchor" aria-label="永久链接：开始使用" href="#getting-started"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Prerequisites</h3><a id="user-content-prerequisites" class="anchor" aria-label="永久链接：先决条件" href="#prerequisites"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">The CfdOF workbench depends on the following external software, some of
which can be automatically installed (see below for instructions).</p>
<ul dir="auto">
<li><a href="https://www.freecadweb.org/downloads.php" rel="nofollow">Latest release version of FreeCAD (at least version 0.20.0 / git commit 29177)</a>
or <a href="https://github.com/FreeCAD/FreeCAD-Bundle/releases/tag/weekly-builds">latest development version (prerelease)</a></li>
<li>OpenFOAM <a href="http://openfoam.org/download/" rel="nofollow">Foundation versions 9-10</a> or <a href="http://openfoam.com/download" rel="nofollow">ESI-OpenCFD versions 2006-2306</a></li>
<li><a href="http://www.paraview.org/" rel="nofollow">Paraview</a></li>
<li><a href="https://sourceforge.net/projects/cfmesh-cfdof/" rel="nofollow">cfMesh (customised version updated to compile with latest OpenFOAM versions)</a></li>
<li><a href="https://hisa.gitlab.io" rel="nofollow">HiSA (High Speed Aerodynamic Solver)</a></li>
<li><a href="http://gmsh.info/" rel="nofollow">Gmsh (version 2.13 or later)</a> - optional, for generating tetrahedral meshes</li>
</ul>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Setting up the CfdOF workbench</h3><a id="user-content-setting-up-the-cfdof-workbench" class="anchor" aria-label="永久链接：设置 CfdOF 工作台" href="#setting-up-the-cfdof-workbench"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Windows</h4><a id="user-content-windows-1" class="anchor" aria-label="永久链接：Windows" href="#windows-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">The latest
<a href="https://www.freecadweb.org/downloads.php" rel="nofollow">release</a>
or <a href="https://github.com/FreeCAD/FreeCAD-Bundle/releases/tag/weekly-builds">development</a>
FreeCAD build can be obtained (64 bit version) and installed
by respectively running the installer or extracting the .7z archive to a directory
&lt;FreeCAD-directory&gt;. In the latter case, FreeCAD can be run in place
(&lt;FreeCAD-directory&gt;\bin\FreeCAD.exe).</p>
<p dir="auto">CfdOF itself is installed into FreeCAD using the Addon manager:</p>
<ul dir="auto">
<li>Run FreeCAD</li>
<li>Select Tools | Addon manager ...</li>
<li>Select CfdOF in the list of workbenches, and click "Install/update"</li>
<li>Restart FreeCAD</li>
<li>For installation of dependencies, see below</li>
</ul>
<p dir="auto">Note: The CfdOF workbench can be updated at any time through the Addon manager.</p>
<div class="markdown-heading" dir="auto"><h5 tabindex="-1" class="heading-element" dir="auto">Dependency installation</h5><a id="user-content-dependency-installation" class="anchor" aria-label="永久链接：依赖安装" href="#dependency-installation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Dependencies can be checked and installed conveniently from the CfdOF Preferences panel in FreeCAD.
In the FreeCAD window, select Edit | Preferences ... and choose "CfdOF".  The dependencies can be installed as
individual components or as part of a docker container (refer to the <strong>Docker container install</strong> section below).</p>
<p dir="auto">The OpenFOAM installation is via the
<a href="https://www.openfoam.com/download/install-binary-windows-mingw.php" rel="nofollow">OpenCFD MinGW package</a>, and
the <a href="https://bluecfd.github.io/Core/" rel="nofollow">BlueCFD Core</a> port of OpenFOAM is also supported.</p>
<p dir="auto">OpenFOAM can be installed manually using the above links, or by clicking the relevant
button in the Preferences panel described above. If you experience problems running OpenFOAM in CfdOF, please make
sure you have a working installation by following instructions on the relevant websites.</p>
<p dir="auto">To interface correctly with the OpenFOAM installation, CfdOF needs to be able to write to its
install location.
Some users experience problems using a location inside C:\Program Files due to restrictions
imposed by Windows User Account Control. It is therefore suggested to install to an alternative
location, preferably in your home directory.</p>
<p dir="auto">If OpenFOAM is installed with administrator privileges using the above packages, then Microsoft MPI
will also optionally be installed. If not, then it will be necessary to download and
install it manually from <a href="https://learn.microsoft.com/en-us/message-passing-interface/microsoft-mpi#ms-mpi-downloads" rel="nofollow">here</a>.
MPI is needed in order to run in parallel.</p>
<p dir="auto">Set the OpenFOAM install directory in the preferences
panel to the install directory ending in the 'vXXXX' subfolder (where XXXX is the version number installed)
for the MinGW package, or the BlueCFD install directory.
It will be automatically detected in the default install
locations.</p>
<p dir="auto">Any version of <a href="https://www.paraview.org/download/" rel="nofollow">ParaView</a> can be installed,
by following the above link or clicking the relevant button in the Preferences panel.
Set the ParaView install path in the preferences panel to the 'paraview.exe' file in the 'bin'
subfolder of the ParaView installation. Common defaults will be detected if it is left blank.</p>
<p dir="auto">Likewise, cfMesh and HiSA can be installed from the Preferences panel. Do not close
it until the 'Install completed' message is received.
Note that the OpenFOAM installation must be in a writable location
for cfMesh and HiSA to be installed successfully.</p>
<p dir="auto">Choosing the "Check dependencies" option will verify that all
prerequisites have been successfully installed.</p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Linux</h4><a id="user-content-linux-1" class="anchor" aria-label="永久链接：Linux" href="#linux-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">AppImages of the latest <a href="https://www.freecadweb.org/downloads.php" rel="nofollow">release</a>
or <a href="https://github.com/FreeCAD/FreeCAD-Bundle/releases/tag/weekly-builds">development</a>
versions of FreeCAD can be downloaded and run directly
without installation. Note that you will
have to enable execution permission on the downloaded file to run it.
Otherwise, FreeCAD can be built
from the source code at <a href="https://github.com/FreeCAD/FreeCAD">https://github.com/FreeCAD/FreeCAD</a> .</p>
<p dir="auto">Note:</p>
<ul dir="auto">
<li>Installations of FreeCAD via Linux package managers
make use of your local Python installation. Therefore you might need to install additional
Python packages to get full functionality. The dependency checker (see below) can help to diagnose
this.</li>
<li>Note that the 'Snap' container installed through some distributions' package managers
can be problematic as it does not allow access to system
directories, and therefore OpenFOAM has to be installed in the user's home directory
to be runnable from FreeCAD.</li>
</ul>
<p dir="auto">For the reasons above we recommend the AppImage as the most robust installation
option on Linux.</p>
<p dir="auto">CfdOF itself is installed into FreeCAD using the Addon manager:</p>
<ul dir="auto">
<li>Run FreeCAD</li>
<li>Select Tools | Addon manager ...</li>
<li>Select CfdOF in the list of workbenches, and click "Install/update"</li>
<li>Restart FreeCAD</li>
<li>For installation of dependencies, see below</li>
</ul>
<p dir="auto">Note: The CfdOF workbench can be updated at any time through the Addon manager.</p>
<div class="markdown-heading" dir="auto"><h5 tabindex="-1" class="heading-element" dir="auto">Dependency installation</h5><a id="user-content-dependency-installation-1" class="anchor" aria-label="永久链接：依赖安装" href="#dependency-installation-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Dependencies can be checked and some of them installed
conveniently from the CFD Preferences panel in FreeCAD.
In the FreeCAD window, select Edit | Preferences ... and
choose "CfdOF".</p>
<p dir="auto">The dependencies can be installed manually, or as part of a docker container (refer to Docker container install below). Manual
installation may be undertaken for OpenFOAM (<a href="https://openfoam.com/download" rel="nofollow">OpenCFD</a> or <a href="https://openfoam.org/download/" rel="nofollow">Foundation</a>
versions), <a href="http://www.paraview.org/" rel="nofollow">Paraview</a> and <a href="http://gmsh.info/" rel="nofollow">Gmsh</a> (optional) by using the links above or your distribution's package
manager. Note, however, that the OpenFOAM packages bundled in
some Linux distributions may be out of date or incomplete; for example,
the standard Debian and Ubuntu packages do not include the build command 'wmake'
and therefore cannot be used with the optional components 'HiSA' and 'cfMesh'.
We therefore recommend installation of the packages supplied through
the official websites above. Please make sure the install the 'development'
package where available (usually named with the suffix '-devel' or '-dev') to
be sure that the optional components 'HiSA' and 'cfMesh' can be compiled
with 'wmake'.</p>
<p dir="auto">Set the OpenFOAM install directory in the preferences
panel - examples of typical install locations are /usr/lib/openfoam/openfoam2306,
/opt/openfoam10 or /home/user/OpenFOAM/OpenFOAM-10.x (it will be automatically
detected in common default install
locations). Note that if you have loaded the desired OpenFOAM
environment already before starting FreeCAD, the install directory should be left blank.</p>
<p dir="auto">cfMesh and HiSA can be installed using the Preferences panel described above,
and can be downloaded and built from their source
code inside your OpenFOAM installation if you have
not already done so yourself. Note that this is a lengthy process.</p>
<p dir="auto">Choosing the "Check dependencies" option will verify that all
prerequisites have been successfully installed.</p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Docker container install</h4><a id="user-content-docker-container-install" class="anchor" aria-label="永久链接：Docker 容器安装" href="#docker-container-install"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Docker containers offer a convenient way of providing pre-compiled program packages for both windows and linux. macOS can also be supported but
assistance will be required to setup a container.  Please leave a message on the <a href="https://forum.freecadweb.org/viewforum.php?f=37" rel="nofollow">forum</a>.</p>
<div class="markdown-heading" dir="auto"><h5 tabindex="-1" class="heading-element" dir="auto">Docker on Windows</h5><a id="user-content-docker-on-windows" class="anchor" aria-label="永久链接：Windows 上的 Docker" href="#docker-on-windows"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">The preferred docker run-time for Windows is via <a href="https://podman.io/" rel="nofollow">podman</a> as currently this provides fast filesystem integration.
<a href="https://www.docker.com/products/docker-desktop/" rel="nofollow">Docker Desktop</a> may also be used.</p>
<ol dir="auto">
<li>Install <a href="https://github.com/containers/podman/releases/download/v4.2.1/podman-v4.2.1.msi">podman</a> (or <a href="https://www.docker.com/products/docker-desktop/" rel="nofollow">docker desktop</a>).</li>
<li>If using podman, open a cmd window and issue the following commands:
<ul dir="auto">
<li><code>podman machine init</code></li>
<li><code>podman machine start</code></li>
<li><code>podman machine set --rootful</code></li>
</ul>
</li>
<li>Edit → Preferences → CfdOF: Press the <em>Install Paraview</em> button.</li>
<li>Edit → Preferences → CfdOF: Select <em>Use docker</em>.</li>
<li>Press the <em>Install Docker Container</em> button. There is no need to install gmsh, cfmesh and HISA as they are included in the docker image.</li>
<li>If using podman, fast WSL file system integration can be enabled:
<ul dir="auto">
<li>Create a new subdirectory (for example <code>cfdof</code>) in the following firectory created by podman:
<code>\\wsl$\podman-machine-default\home\user</code></li>
<li>In the cfdof preference page, set the default output directory as above:
<code>\\wsl$\podman-machine-default\home\user\cfdof</code></li>
</ul>
</li>
<li>Press the <em>Run dependency checker</em> button.</li>
</ol>
<div class="markdown-heading" dir="auto"><h5 tabindex="-1" class="heading-element" dir="auto">Docker on Linux</h5><a id="user-content-docker-on-linux" class="anchor" aria-label="永久链接：Linux 上的 Docker" href="#docker-on-linux"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="auto">
<li>Install docker using these <a href="https://www.linuxtechi.com/install-docker-engine-on-debian/" rel="nofollow">instructions</a> (or similar).</li>
<li>Install paraview as per the package installation instructions for your distribution
(for example <code>sudo apt-get install paraview</code> on debian).</li>
<li>Edit → Preferences → CfdOF: Select <em>Use docker</em>.</li>
<li>Press the <em>Install Docker Container</em> button. There is no need to install gmsh, cfmesh and HISA as they are included in the docker image.</li>
<li>Press the <em>Run dependency checker</em> button.</li>
</ol>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Documentation</h2><a id="user-content-documentation" class="anchor" aria-label="永久链接：文档" href="#documentation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">At present there is no formal documentation for CfdOF apart from this README.
However, demonstration cases
are provided inside the 'Demos' folder of the
<a href="https://github.com/jaheyns/cfdof">CfdOF workbench directory</a>. These aim
to provide a basic overview of features and best practices. The examples are run
by loading and executing the macro files ending in '.FCMacro' in the various sub-directories
in the 'Demos' directory. Where there are several numbered files, these should be run in order
and aim to demonstrate step-by-step how the case is set up.</p>
<p dir="auto">Community assistance may be sought at the
<a href="https://forum.freecadweb.org/viewforum.php?f=37" rel="nofollow">CfdOF dedicated FreeCAD forum</a>,
and a list of various third-party documentation is available in
<a href="https://forum.freecadweb.org/viewtopic.php?f=37&amp;t=33492#p280359" rel="nofollow">the following forum post</a>.</p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">FAQ</h3><a id="user-content-faq" class="anchor" aria-label="永久链接：常见问题解答" href="#faq"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Q: Do I have to create a watertight geometry?</p>
<p dir="auto">A: This isn't necessary if using the cartesian mesh generators <em>snappyHexMesh</em> and <em>cfMesh</em>.
You can make use of shells and compounds instead of creating solids, as long as the
collection of shapes in the compound being meshed blocks off the volume desired.
Gaps smaller than the mesh spacing are also allowed.</p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Feedback</h2><a id="user-content-feedback" class="anchor" aria-label="永久链接：反馈" href="#feedback"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Reporting Bugs</h3><a id="user-content-reporting-bugs" class="anchor" aria-label="永久链接：报告错误" href="#reporting-bugs"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">Please discuss issues on the <a href="https://forum.freecadweb.org/viewforum.php?f=37" rel="nofollow">CfdOF FreeCAD forum</a>
for community assistance.
Bugs can be reported on the <a href="https://github.com/jaheyns/cfdof">Github project site</a>.</p>
<p dir="auto">Please first read the <a href="https://forum.freecadweb.org/viewtopic.php?f=37&amp;t=33492#p280359" rel="nofollow">guidelines for reporting bugs</a>
in order to provide sufficient information.</p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Development</h2><a id="user-content-development" class="anchor" aria-label="永久链接： 发展" href="#development"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">If you would like to get involved in the development of CfdOF, please refer to the <a href="/jaheyns/CfdOF/blob/master/CONTRIBUTING.md">Contribution guidelines</a>
and <a href="/jaheyns/CfdOF/blob/master/ROADMAP.md">Roadmap</a>.</p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto">Acknowledgements</h2><a id="user-content-acknowledgements" class="anchor" aria-label="永久链接：致谢" href="#acknowledgements"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Funding</h3><a id="user-content-funding" class="anchor" aria-label="永久链接：资金" href="#funding"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">This development was made possible through initial funding from <a href="http://www.eskom.co.za" rel="nofollow">Eskom Holdings SOC Ltd</a>
and the <a href="https://www.csir.co.za" rel="nofollow">Council for Scientific and Industrial Research</a> (South Africa).</p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto">Contributors</h3><a id="user-content-contributors" class="anchor" aria-label="永久链接：贡献者" href="#contributors"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li>Oliver Oxtoby (CSIR, 2016-2018; private 2019-) <a href="mailto:oliveroxtoby@gmail.com">oliveroxtoby@gmail.com</a></li>
<li>Johan Heyns (CSIR, 2016-2018) <a href="mailto:jaheyns@gmail.com">jaheyns@gmail.com</a></li>
<li>Alfred Bogaers (CSIR, 2016-2018) <a href="mailto:alfredbogaers@gmail.com">alfredbogaers@gmail.com</a></li>
<li>Jonathan Bergh (2022)</li>
<li>Qingfeng Xia (2015)</li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">托马斯·施拉德 (2017-) </font></font><a href="mailto:info@schraderundschrader.de"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">info@schraderundschrader.de</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">迈克尔·欣德利 (2016)</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">马克·麦肯齐（CNF，2022）</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">凯蒂·阿克马尔 (2022) [论坛：@KAKM]</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">阿德里安·因绍拉尔德 (2022)</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">克劳斯·森布里茨基 (2017)</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">奉献精神</font></font></h3><a id="user-content-dedication" class="anchor" aria-label="永久链接： 奉献" href="#dedication"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">CfdOF 致力于纪念迈克尔·欣德利 (Michael Hindley)。正是由于他对 FreeCAD 和开源软件不可抑制的热情，这个工作台才得以存在。安息。</font></font></p>
</article></div>
