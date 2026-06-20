---
title: "Peregrine Falcons and Blue Whales"
date: 2019-11-04T20:00:00+05:30
description: "A post detailing why the world's supposed fastest animal is a fraud."
url: /blog/2019/11/04/whales.html
math: true
---

If you Google the world's fastest animal, you will find that the peregrine falcon is considered to top the speed charts. According to National Geographic, it can hit maximum speeds of 200 miles per hour while diving. However, if we are using the metric of the fastest an animal can go in free fall, why not take it to the extreme?

The maximum speed an object can reach in free fall, called its **terminal velocity**, is primarily determined by two things: shape and weight. While the shape of the peregrine falcon is very much streamlined, it is not particularly heavy. This is where the blue whale comes in. While not the most streamlined of objects a blue whale is still extremely massive. Thus, we would expect that it could potentially beat the peregrine falcon in terminal velocity, claiming the title of world's fastest animal. So let's calculate it!


First let's take a look at the drag equation (with the linear term approximated away):

\[
F_d =  \frac{1}{2} A \rho v^2 C_d
\]

This looks sort of complicated at first, so let's break it down. First, \( F_d \) is the drag force the air exerts on a moving object, thus opposing its motion. \( A \) is the front-facing area of the object, \( \rho \) is the density of what the object is moving through (usually air), and \( v \) is its velocity. Finally, \( C_d \) is the drag coefficient of the object, which is based on it's shape and describes how aerodynamic the object is.

Next let's look at the force of gravity, \( F_g \). For objects relatively near Earth's surface, this is:

\[
F_g = mg
\]

The \( m \) represents the mass of the object and the \( g \) represents the acceleration due to gravity at the Earth's surface. Since when an object is at terminal velocity the force of gravity pulling the object downwards is equal to the resistance of the air pushing back upwards, we can make the following statements:

\[
F_d = F_g \\
\frac{1}{2} A \rho v^2 C_d = mg
\]

Now, with some algebra, we can rearrange the equation into the following form to get our terminal velocity:

\[
v = \sqrt{\frac{2 m g}{A \rho C_d}}
\]

Using standard SI units (meters, kilograms, etc.) and looking up the density of air at sea level and mass of a blue whale online, we can express the values \( g=9.8 \mathrm{m/s/s} \), \( m = 120,000 \mathrm{kg} \), \( \rho = 1.2 \mathrm{kg/m^3} \), \( A = \pi d^2 / 4 = \pi (4.4 \mathrm{m})^2 / 4 = 15.2 \mathrm{m^2} \).

As it is really hard to obtain the drag coefficient for a blue whale without sticking one (or a model thereof) in a wind tunnel and taking some measurements, I'm going to do what all experimental physicists love doing: an approximation. Given our hypothetical whale will be diving head first, the front kind of looks like a sphere if you squint and stand on your head. Thus we will assume it is one (which honestly probably won't lead to us being extremely far off, and definitely will give an underestimate for terminal velocity, which might be good enough).

Given \( C_d = 0.47 \) for a sphere in turbulent airflow, and plugging this all in, we get the terminal velocity of a blue whale is:

\[
v = 524 \mathrm{m/s} = 1172 \mathrm{mph}
\]

That's more than 1.5 times the speed of sound, and much faster than the puny 200mph of the peregrine falcon!

Realistically, this would be even faster, as a blue whale diving downwards face first would be much more streamlined than an average sphere (assuming it didn't flop around too much). Perhaps I will build a rudimentary wind tunnel and test this at a later date. Another thing we overlooked for simplicity was the density of air changing with altitude, but what we really care about is the whale's maximum velocity near sea level, so this is a fair approximation.

So, it may not even be practical to lift one into the upper atmosphere and drop it directly downwards (unless it magically appeared in the sky next to a bowl of petunias[^1]), but *technically* the blue whale's maximum velocity is far greater than that of the peregrine falcon, making it the fastest animal in the world. While **I very much acknowledge that this is an entirely unreasonable viewpoint and completely disregards biology (while making some vast approximations as well)**, I still claim the fact that you read all the way through this post and may (or may not) have learned some physics is at least worth something.

[^1]: See *A Hitchhiker's Guide to the Galaxy* by Douglas Adams

---
###### © 2019 Noah Paladino
