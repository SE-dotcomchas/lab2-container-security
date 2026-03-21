# lab2-container-security
Hello there this is my second assignment that i am turning in for the course. What i did was that i first created a app riddled with vunerabilities
and created a trivy scan to see just how exploitable the app was. then afterwards i made a second version that was a more simple and newer version of python
that is significantly harder to exploit. Afterwards the file size difference between the two was enourmus with the exploitable app being more then a 1gb big and the hardened one slightly more then 200 which is massive difference. It also did not have hundreds of vunerabilities unlike the predecessor after making a trivy scan
here is a image of before and after to make it clear

First Version https://github.com/SE-dotcomchas/lab2-container-security/blob/main/Images/a1ed584bd68cc68ffd83acf381ed4ccd.png
Second Version after hardening  https://github.com/SE-dotcomchas/lab2-container-security/blob/main/Images/fa3d9101ab7da3ecc83f9eb3a34f48c3.png

I also generated a so called SBOM which is a useful tool to see what your app uses and to potentially find new weaknesses in the app.
the reason for it is that it is quite important to know what dependecies your application has in order to be able to determine if something is out of date
for example.

----------------------------------------------------------------------------------------------------------------------------------------

The second thing i did for the lab was to try out gatekeeper to see how it would refuse to deploy unsafe pods that can be easely exploited meanwhile
an app that is secure is allowed to be ran.

Below here is a image how it looks when i try to deploy both safe and unsafe pods

Unsafe pod https://github.com/SE-dotcomchas/lab2-container-security/blob/main/Images/ca2859cf0fd3ddaee43f9201e2abf2be.png

Safe pod  https://github.com/SE-dotcomchas/lab2-container-security/blob/main/Images/89ec23a1b3c2687eb48b2de32f4ee396_1.png

------------------------------------------------------------------------------------------------------------------------------------------

Reflection

So after having done everything now i can safely say that hardening is not that hard it and it is 100% essential to do
to keep your applications safe and secure. I also now understand that all applications that you use are important to keep it safe. like protecting yourself
from deploying bad insecure pods. catching critical vunerabilitys and generating the SBOM, etc. As long as you secure the entire pipeline the odds of releasing bad code will drasticly go down which should be quite easy to do. i would rather not have a CEO or a manager breathing down your neck after launching a new version
of an app with a critical flaw afterall


