> ["I'd rather write code than papers."](https://www.cwi.nl/en/stories/interview-guido-van-rossum-201cid-rather-write-code-than-papers201d/) 
> - Guido van Rossum

## Ramūnas Girdziušas' Projects

aabbtree77 at gmail.com

[CV (React Show-off)](https://aabbtree77.github.io/cv/), [resume.pdf](https://aabbtree77.github.io/pdfs/RamunasGirdziusasResume.pdf), [cv.pdf](https://aabbtree77.github.io/pdfs/RamunasGirdziusasCV.pdf)

<div style="display: flex; justify-content: flex-start">
  <div style="font-size: 1rem;">Last Update: December 2024</div>
</div>

I studied electrical engineering in Lithuania from 1994 to 1999, followed by research in machine learning in Finland from 2000 to 2008.

Later I did three postdoc projects and came back to where I belong ;). 

My goal is to become a [software engineer](https://1x.engineer/) as I am mostly interested in programming languages and engineering systems. Without a compiler everything is unnecessarily hard: [algebra](https://aabbtree77.github.io/tensors/), computer science metanotation, uncodified business processes...

An ideal work for me is a rewrite and downscaling, preferably in something static and GC-based.

Take a look at some of my work in [embedded software](https://github.com/aabbtree77/adast), [IoT](https://github.com/aabbtree77/esp32-vpn), [3D](https://github.com/aabbtree77/twinpeekz2), and [webdev](https://github.com/aabbtree77/law2).

# Selected Projects

## Work in Progress

Vilnius, Now.

Still learning some ways to build web GUIs and services. My interim release includes [backend](https://github.com/aabbtree77/auth-starter-backend) and [frontend](https://github.com/aabbtree77/auth-starter-frontend) for a 3rd party-free user authentication.

## [lawtrust.eu](https://lawtrust.eu/): [lawlt.eu](http://www.lawlt.eu/) [Improved](https://github.com/aabbtree77/law2)

Vilnius, February 2024.

A multilingual website for a lawyer who speaks nine languages. Static HTML, Tailwind CSS, [gomarkdown](https://github.com/gomarkdown/markdown), porkbun.com, and github pages.

## [Web-Log](https://github.com/aabbtree77/miniguestlog)

Vilnius, 2023-2024.

A MERN app to [log](https://aabbtree77.github.io/miniguestlog/loadGuestsSpinner.html) geolocation of the last 50 visitors of this homepage. MongoDB Atlas, Compass, render.com, github pages, ipify.org, and geoip-lite API for the GeoLite data from MaxMind.

It took me about a week or two to cobble up everything and get a fully working web app with the help of ChatGPT. A month at most with learning. Then I started reading that Js is not good, use TypeScript instead, MongoDB was a mistake, SQLite vs PostgreSQL. A year later not much is done and I am still figuring out "the right way" around 3-5 Js/Ts runtimes, eleven build systems, two module types, frameworks and metaframeworks, caching, React (TanStack) Query vs server components, React router vs Next.js routers, endless databases, DDOS, JWT vs session cookies, passwords or OAuth 2, and on and on it goes.

When someone tells you "we got it right this time"... it feels like that hammer scene from Oldboy (2003) when an elevator door opens.

## [Paper Guillotine](https://github.com/aabbtree77/adast)

Vilnius, 2020 - 2024.

A joint work with Saulius Rakauskas (Infovega). We have been maintaining a real factory machine since February 2020 (last update: February 2024). I wrote microcontroller code in C (avr-gcc). The only really useful code that I wrote in my entire career so far. Zero stars, downloads, citations, and yet it improved the daily lives of factory workers.

Comparing this project and my work in France to the endless "life searches", the major conclusion is that I am miserable when I am left to my own devices. It is much better to work in a tandem.

## [P2P Connectivity](https://github.com/aabbtree77/esp32-vpn)

Vilnius, 2021 - 2022.

A joint work with Saulius Rakauskas (Infovega): A remote plant watering system with ESP32, MicroPython, Mosquitto MQTT, Ubuntu and [awl](https://github.com/anywherelan/awl) with golibp2p. Numerous tests of [hole punching](<https://en.wikipedia.org/wiki/Hole_punching_(networking)>) through layers of routers with the use of the P2P network other than torrents, to control an ESP32 device globally, without obscure 3rd party services.

The technology is there, but the killer app is not, as always. In a way, this is about downscaling the ESP RainMaker. Building something that approximates an opaque communication system out of basic well-known FOSS blocks which can be isolated and controlled when "the shit hits the fan". 

Nowadays (two years later) I would remove the ESP32 part almost entirely and go for the embedded Linux boards instead. Life is too short for anything non-Linux. A recent Indian Morse code broadcasting ring on a finger deserves to be mentioned in the Appendix section on the applications of low RAM devices.

## [Volumetrically-Lit Sponza (Go, Nim)](https://github.com/aabbtree77/twinpeekz2)

Vilnius, 2020 - 2022.

Implemented volumetric lighting in [Go](https://github.com/aabbtree77/twinpeekz) and [Nim](https://github.com/aabbtree77/twinpeekz2) (forward rendering, shadow mapping, PBR, 3D ray marching, OpenGL) following [Balázs Tóth, Tamás Umenhoffer (2009)](https://diglib.eg.org/handle/10.2312/egs.20091048.057-060), and [Tomas Öhberg (2017)](https://gitlab.com/tomasoh/100_procent_more_volume).

Note: This is a real time rendering pipeline which combines multiple stages and makes sure everything fits into 16ms frames. It will save a lot of time for someone who wants to start building a 3D engine while being lost at downscaling any existing ones. The code includes neither ECS, nor physics, which could be a pro. One of my goals was also to test the impact of Go's garbage collector in real time rendering. 

OpenGL, Vulkan, or WebGPU? Gave up on this, but note that they all spread the state, and the languages we use are not designed for these backends at all. RenderDoc is essential, but this is virtually like writing in Assembly. Reddit votings indicate that Vulkan is still less used than OpenGL, but it already helps to run [d3d9-d3d11 on Linux](https://github.com/doitsujin/dxvk/issues/3789). OpenGL still has a serious advantage due to ["Learn OpenGL"](https://learnopengl.com/). Can one do Vulkan with ChatGPT?

## [The Algebra of Tensor Fields](https://aabbtree77.github.io/tensors/)

Vilnius, 2015 - 2024.

Verified tensor algebras of Donn G. Shankland (1970). Spinors are left as an exercise for the reader ;). Feel free to include the PCT transforms, gauge invariance, "GR frames", multiple particles, extend this to higher dimensional space-times...

["Après la montagne, il y a la montagne..." &#8722; Desireless, Hari om Ramakrishna (1989)](https://www.youtube.com/watch?v=18rZv8qWZqA)

## [MNIST-0.17 (Python)](https://github.com/aabbtree77/MNIST-0.17)

Vilnius, 2014 - 2015.

Confirmed that Jonas Matuzas' CNN model is one of the most convincing results in the MNIST digit recognition. Built my own kriging and Adam Coates et al. features-based "autoML" image recognition system which was sound, but not competitive enough. It relied on the block-Choleski inverse of a large covariance matrix which may not fit into 64GB RAM. It was hyperparameter-free as I learned in France it was better to estimate the variance parameter in the Gaussian kernel quickly from the sample of data instead of running the whole gradient ascent on the maximum likelihood. However, such simple and reliable systems are hard to scale beyond O(100K) vectors. It had the error rates inferior to those of the CNNs (85% CIFAR-10 accuracy vs world records reaching over 99%).

A big problem that a lot of us have not noticed for a long time is what Carl Hewitt would describe as "The ideology took its turn". It was hard not to believe in that

**Linear is better than quadratic, polynomial, nonlinear, or multilayer-nonlinear?**

It turns out that `linear` is actually `cubic` and demands at least `float64`, while the SGD with convolutions does not even need `float32`, not to mention the error rates which is the essence of the game.

## [3D Shape Normalization (Matlab)](https://diglib.eg.org/handle/10.2312/3dor.20141044.009-015)

PostDoc Chronicles 3: Lugano, 2013-2014. My second encounter with quadratically-constrained quadratic cost optimization, where I have mapped the "Swiss Roll" problem to the fast multipole method-based electrostatics with an approximate distance
constraint handling (simple projections ala Karmarkar and Cimmino in linear algebra). Davide Boscaini implemented the constraint gradient exactly and pushed the error rates.

The lab was interesting in that everybody was forced to learn at least a bit of the "Einsteinian motif" to consider equations on a surface or a graph. We used some tools to clean 3D meshes which was very liberating considering omnipresent Matlab. Randolf Schärfig was developing his 3D engine in C++ nearby in the same hall of cubicles.

I wasted a lot of time trying to apply the MDS-like algorithms on the [Protein Data Bank](https://www.rcsb.org/), thinking of the data set myopically as some low-level filtering problem. Little I knew that at the same time AlphaFold was already being developed...

We are often just a few steps away from something great. In my case, I missed the DNA sequence data (being narrow minded and more into physics while totally ignoring chemistry and biology), and also could not overcome the belief that neural net convolutions will work well only on the continuous data. 

## [Cloud Computing (Scilab)](https://hal.archives-ouvertes.fr/hal-00723427)

PostDoc Chronicles 2: Saint-Étienne, 2012-2013.

Optimization of the fluid flow which was implemented before me with OpenFOAM, CATIA, STAR CCM+ and ParaView, running on the ProActive PACA Grid cloud (INRIA) via the Scilab-to-Java bridge managed by Fabien Viale. The optimization involved kriging and CMA-ES as the meta-optimizer of the expected multi-point improvement whose MC integration I sped up with a specialized unscented transform. See the [slides](https://github.com/aabbtree77/aabbtree77.github.io/blob/main/pdfs/optimization2012.pdf).

Note: David Ginsbourger approached the integral differently, reducing it to Fortran routines that needed to compute "only" multivariate Gaussian quadratures. 

This was one of the best projects in my life. So many things came together.

## [Modified Thomson Problem (Unpublished)](https://github.com/aabbtree77/aabbtree77.github.io/blob/main/pdfs/ucla2009.pdf)

PostDoc Chronicles 1: Los Angeles, 2008-2009.

The modified Thomson problem is a quadratically-constrained quadratic cost with deceptively simple constraints. I performed linearization and spectral analysis leading to a few definite statements. They did not become a larger research program.

## [Anisotropic Diffusion Filters](https://aaltodoc.aalto.fi/handle/123456789/2999)

My DSc (PhD) thesis, Espoo 2002-2008.

Added a layer of model selection to discontinuity-preserving filtering. Guided by Dr. Jorma Laaksonen and Prof. Erkki Oja.

Daffertshofer-Haken-1994 as a strategically wrong, but inspiring paper, E.T. Jaynes, machine learning in 2000s, my great nine years in Finland: Suomenlinna, Serena... Vaida Rutkauskaitė, Alexander Ilin, Vitaliy Nevdacha, Mykola Ivanchenko, Elia Liitiäinen, Jan-Hendrik Schleimer, Jarrod Creado, Leo Michael, Jaakko Martti Johannes Miettinen, Ville Rantamaula, Dexter He, Mikko Katajamaa, Petteri Räisänen, Jaakko Peltonen, Petri Hyötylä, Matthieu Molinier, Jagdeesh Rajani, Sandro Grech, Ivan Ore, Giedrius Zavadskis, Anita Bisi, Sergej Doudorov, Maxim Govtva, Paola Huaynate... I remember you.

## UNIPEN Parser (Matlab)

May 2000.

My first job. At the CIS Lab, Helsinki University of Technology (TKK), guided by Dr. Jorma Laaksonen. During the first two weeks I wrote a parser which loaded UNIPEN data into Matlab. It was a non-recursive use of fscanf for the internal (CIS lab-specific) subset of UNIPEN.

<br>

<table align="center">
    <tr>
    <th align="left">Ilya Kabakov. The Man Who Flew into Space from his Apartment, 1988</th>
    </tr>
    <tr>
    <td>
    <img src="imgs/IljaKabakov1986.jpg"  alt="Modern art, USSR" width="100%" >
    </td>
    </tr>
</table>

<br>
