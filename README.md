> "Let it go. We have bigger fights."  
> \- Reacher (2022)

# My Projects

Ramunas Girdziusas, aabbtree77 at gmail.com

[CV (React show-off)](https://aabbtree77.github.io/cv/), [resume.pdf](https://aabbtree77.github.io/pdfs/RamunasGirdziusasResume.pdf), [cv.pdf](https://aabbtree77.github.io/pdfs/RamunasGirdziusasCV.pdf)

I studied electrical engineering in Lithuania from 1994 to 1999, researched machine learning in Finland from 2000 to 2008, completed three postdoc projects, and returned in 2014 with the goal to become a [software engineer](https://1x.engineer/).

Take a look at some of my work in [embedded software](https://github.com/aabbtree77/adast), [IoT](https://github.com/aabbtree77/esp32-vpn), [3D](https://github.com/aabbtree77/twinpeekz2).

## Work in Progress

Vilnius, Now.

This interim release includes [backend](https://github.com/aabbtree77/auth-starter-backend) and [frontend](https://github.com/aabbtree77/auth-starter-frontend) for a 3rd party-free username/password authentication. It uses TypeScript for the both, and includes a small memo how to set up browser cookies locally and with the HTTPS.

## [lawtrust.eu](https://lawtrust.eu/): [lawlt.eu](http://www.lawlt.eu/) [Improved](https://github.com/aabbtree77/law2)

Vilnius, February 2024.

A multilingual website for a lawyer who speaks nine languages. Static HTML, Tailwind CSS, [gomarkdown](https://github.com/gomarkdown/markdown), porkbun.com, and github pages.

This project was an eye opener about what the SEO and fair search mean in practice:

- [http://www.lawlt.eu/](http://www.lawlt.eu/) - Built around 2012, the HTTP, data inside the PHP CMS called "CMS Made Simple". Google was paid to advertise it on search.

- [https://lawtrust.eu/](https://lawtrust.eu/) - Built in 2024, the HTTPS, data directly inside the HTML hosted on github.com. Github is owned by Microsoft. Google was never paid to advertise it.

The search for "lawyer vilnius" (January 13th, 2025):

- Google: lawlt.eu - Page 3, lawtrust.eu - Page 13.

- Bing: lawlt.eu  - no results in the first 20 pages, lawtrust.eu - Page 1!

- DuckDuckGo: lawlt.eu  - no results in the first 20 pages, lawtrust.eu - Page 1!

## [Web-Log](https://github.com/aabbtree77/miniguestlog)

Vilnius, 2023-2024.

A MERN app to [record](https://aabbtree77.github.io/miniguestlog/loadGuestsSpinner.html) geolocation of the last 50 visitors of aabbtree77.github.io. MongoDB Atlas, Compass, render.com, github pages, ipify.org, and geoip-lite API for the GeoLite data from MaxMind.

It took me about a week or two to cobble up everything and get a fully working web app with the help of ChatGPT. 

Then I started looking for "the right way" since MERN is supposedly obsolete. A year has passed, and now I am only lost more than ever.

When someone tells you "we got it right this time"... remember the protagonist's face in the hammer scene from Oldboy (2003), when the elevator door opens.

## [Paper Guillotine](https://github.com/aabbtree77/adast)

Vilnius, 2020 - 2024.

A joint work with Saulius Rakauskas (Infovega). We have been maintaining a *real* factory machine since February 2020 (last update: February 2024). I wrote microcontroller code in C (avr-gcc).

## [P2P Connectivity](https://github.com/aabbtree77/esp32-vpn)

Vilnius, 2021 - 2022.

A joint work with Saulius Rakauskas (Infovega): A remote plant watering system with ESP32, MicroPython, Mosquitto MQTT, Ubuntu and [awl](https://github.com/anywherelan/awl) with golibp2p. Numerous tests of [hole punching](<https://en.wikipedia.org/wiki/Hole_punching_(networking)>) through layers of routers with the use of the P2P network other than torrents, to control an ESP32 device globally, without obscure 3rd party services.

I would remove the ESP32 and focus more on the embedded Linux boards now (2025).

## [Volumetrically-Lit Sponza (Go, Nim)](https://github.com/aabbtree77/twinpeekz2)

Vilnius, 2020 - 2022.

Volumetric lighting in [Go](https://github.com/aabbtree77/twinpeekz) and [Nim](https://github.com/aabbtree77/twinpeekz2) (forward rendering, shadow mapping, PBR, 3D ray marching, OpenGL) following [Balázs Tóth, Tamás Umenhoffer (2009)](https://diglib.eg.org/handle/10.2312/egs.20091048.057-060), and [Tomas Öhberg (2017)](https://gitlab.com/tomasoh/100_procent_more_volume).

The code is a complete rendering pipeline which may save time for someone who wants to start building a 3D engine while being lost at downscaling any existing ones. The code includes neither ECS, nor physics, which could be a pro. One of my goals was also to test the impact of Go's garbage collector in real time rendering. 

[OpenGL, Vulkan, or WebGPU?](https://www.youtube.com/watch?v=MYi-wpcy0h0&ab_channel=JonathanBlowClips) Gave up on this, but note that they all spread the state, and the languages we use are not designed for these backends at all. RenderDoc is essential. Reddit votings indicate that Vulkan is still less used than OpenGL, but it already helps to run [d3d9-d3d11 on Linux](https://github.com/doitsujin/dxvk/issues/3789). OpenGL still has a serious advantage due to ["Learn OpenGL"](https://learnopengl.com/).

## [The Algebra of Tensor Fields](https://aabbtree77.github.io/tensors/)

Vilnius, 2015 - 2024.

Verified tensor algebras of Donn G. Shankland (1970) and abandoned theoretical physics. Theory is no longer compressing anything. It is healthier to trace significant experiments as they appear historically. This could be the only way out of this arXiv madness.

["Après la montagne, il y a la montagne..." &#8722; Desireless, Hari om Ramakrishna (1989)](https://www.youtube.com/watch?v=18rZv8qWZqA)

## [MNIST-0.17 (Python)](https://github.com/aabbtree77/MNIST-0.17)

Vilnius, 2014 - 2015.

Confirmed that Jonas Matuzas' CNN model is one of the most convincing results in the MNIST digit recognition. 

It is such a tragicomedy to observe how GPUs have removed so much theory. The importance of linearity, continuity, precise inverses? The whole classical statistics. Float64, FFT, HMMs, Leo Breiman's trees, Vladimir Vapnik and kernel methods, Variational Bayes, PAC learning, second order/entropy/curvature methods, convergence analysis, numerical/stability analysis, Kolmogorov - Kůrková theorems, cellular neural networks, RNNs, PCA/ICA-based recommendation systems? The whole "auto tune" direction based on hyperparameter optimization also not that useful. 

Instead, the GPU bottleneck analysis, Torch expression compiling, large GPU platforms, experiment planning. Still far from [big meaning](https://youtu.be/gTAghAJcO1o?t=167), horrible at math, physics, 3D backends, web APIs, but we have a few promising directions: Lc0, AlphaFold, Stable Diffusion, ChatGPT/DeepSeek/Grok...

## [3D Shape Normalization (Matlab)](https://diglib.eg.org/handle/10.2312/3dor.20141044.009-015)

PostDoc Chronicles 3: Lugano, 2013-2014. My second encounter with quadratically-constrained quadratic cost optimization, where I have mapped the "Swiss Roll" problem to the fast multipole method-based electrostatics with an approximate distance
constraint handling (simple projections ala Karmarkar and Cimmino in linear algebra). Davide Boscaini implemented the constraint gradient exactly and pushed the error rates.

I wasted a lot of time trying to apply the MDS-like algorithms on the [Protein Data Bank](https://www.rcsb.org/), coding things in C, thinking of the data set myopically as some low-level filtering problem which supposedly needed scaling. Little I knew that at the same time AlphaFold was already being developed... 

## [Cloud Computing (Scilab)](https://hal.archives-ouvertes.fr/hal-00723427)

PostDoc Chronicles 2: Saint-Étienne, 2012-2013.

Optimization of the fluid flow which was implemented before me with OpenFOAM, CATIA, STAR CCM+ and ParaView, running on the ProActive PACA Grid cloud (INRIA) via the Scilab-to-Java bridge managed by Fabien Viale. The optimization involved kriging and CMA-ES as the meta-optimizer of the expected multi-point improvement whose MC integration I sped up with a specialized unscented transform. See the [slides](https://github.com/aabbtree77/aabbtree77.github.io/blob/main/pdfs/optimization2012.pdf).

David Ginsbourger approached the integral differently, reducing it to Fortran routines which needed to compute "only" multivariate Gaussian quadratures. 

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

My first job. At the CIS Lab, [Helsinki University of Technology (TKK)](https://en.wikipedia.org/wiki/Helsinki_University_of_Technology), guided by Dr. Jorma Laaksonen. During the first two weeks I wrote a parser which loaded the CIS Lab-collected UNIPEN data to Matlab.

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
