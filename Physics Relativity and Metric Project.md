
# General Relativity and The Metric Tensor

The metric tensor is the essence of general relativity, and almost all calculations related to general relativity involve the metric tensor. But before we talk about the metric tensor, let's take a brief look at what general relativity is about and why it was created.

## Why was General Relativity Introduced

### Fixing Newton's Gravity

Before the 1900s, Newtonian physics was thought to be the way the universe functions. In Newtonian physics, gravity is a force exerted on a mass by another, just like how if I push someone, I would exert a force on that person.
$$
\vec{F}=m\vec{a}
$$
$$
F=\frac{GMm}{r^2}
$$
By conducting experiments, people could verify that gravity is a force that causes acceleration of objects. However, there is a slight problem. A person can always feel a force, but one cannot feel gravity unless they are touching the ground. Also, the orbits of certain astronomical objects like the Mercury do not follow the path predicted using Newtonian gravity. Physicists mostly ignored these errors because they thought they might be able to resolve them soon.

After the Michelson-Morley Experiment, Newton's laws were being questioned by physicists across the globe, and no one could create a theory that explained the results of the Michelson-Morley Experiment. Mathmatician Hendrik Lorentz used Maxwell's equations and derived time dilation and length contraction, but he dismissed them because those ideas seemed ridiculous.

### Extending the Special Relativity

In 1905, Albert Einstein created the Theory of Special Relativity, which included time dilation and length contraction due to relative uniform motion. It seemed to be a very probable theory.

Because of the success on Special Relativity, Einstein reminded the physics community that Newtonian Physics could not explain gravity. Einstein's Special Relativity also could not explain gravity since objects don't seem to move at constant velocity in a gravitational field.

In 1907, Einstein realized that the theory of Special Relativity could be extended to include gravity. He argued that free fall is the same as inertial movement, and thus Special Relativity must apply to objects that are freefalling. In 1911, Einstein added on to his 1907 article and said that a person would feel gravity if they are in a uniformly accerlerating box in space. Thus, he concluded that these two situations are identical. This is called the equivilance principal. Also, by using special relativity, Einstein stated that the clock on the front-end of the accelerating box ticks faster than the one on the rear-end. 

In the next few years, Einstein encoutered a lot of problems in his theory, and the math he calculated did not agree with his happiest thought. In 1915, Einstein finally completed his General Theory of Relativity, which is really just the Theory of Special Relativity Plus Gravity.

## Einstein's "Gravity" 

### Why Time is More Influencial Than Space

Ok, let's talk a bit about Einstein's quote-unquote "Gravity". In his theory, gravity is caused by both the bending of space and time. However, time dilation has a significantly greater effect than the bending of space.

We know that space and time are intertwined. Also, we know that the more you move in space, the less you move in time, and vice versa. Since we are moving relative to the Earth at neglegable speeds through space compared to the speed of light, time has an exponentially higher impact on us than space does.

### So How Do We Fall Through Time

Here is one way to think about this:
**Objects further away from the Earth's surface travel through time faster and space slower, and on the other hand, objects closer to the Earth's surface travel through time slower and space faster.** This means that objects quote-unquote "trade" their slow speed through space and high speed through time to slow speed through time and high speed through space. This causes them to fall towards the Earth and move faster over time, which explains the $9.81m/s^2$ acceleration calculated by Newton.
This is cool and all, but you might be asking, why would objects want to fall to places with slower ticking time?
Imagine you have a clock on your head and on your feet. If you are floating above the Earth and your body is paralell to the Earth surface's normal vector, the clock on your head would tick slightly faster than the one on your feet. This means that your head is being dragged down when time flows, just like a torque. This is the reason that you fall to the Earth as time passes by.

This is very different from Newtonian gravity, but it's also similar in the sense that the quote-unquote "falling" object is always moving faster as time passes. In Newtonian physics, this is acceleration, and in relativistic physics, this is the trade between speed in time and space.


## The Metric Tensor
Ok, enough about that, let's talk about the metric tensor now.
Briefly speaking, the metric tensor in mathematics allows you to represent one surface with that of another.

Before we dive into the Metric Tensor, let me first introduce and review some core mathematical concepts needed. 

## 1. What is a Matrix
A matrix is a 2d array of numeric or expressional values. It can look like this:

$$
\begin{bmatrix}
x & 9.2 \\
{\frac {3\pi} 4} & -12
\end{bmatrix}
$$

Or this:

$$
\begin{pmatrix}
1 & 2\\
9 & 8
\end{pmatrix}
$$

It has no meaning by itself -- it's just a way of arranging and visualizing variables. Each number or variable or expression in the matrix is called an "entry" or "element".
***
In mathematics, a matrix acts like any other variables/values. All the basic operations like addition and multiplication apply to the matrix. For instance, the operation "entry wise matrix addition" looks like this:

$$
\begin{bmatrix}
1 & 2\\
9 & 8
\end{bmatrix}
+
\begin{bmatrix}
4 & -9\\
-6 & 13
\end{bmatrix}
{=}
\begin{bmatrix}
5 & -7\\
3 & 21
\end{bmatrix}$$

Basic matrix multiplication looks like this.[^1]
$$
\begin{bmatrix}
1 & 9\\
3 & -12
\end{bmatrix}
\times
\begin{bmatrix}
4 & 2\\
-5 & -2
\end{bmatrix}
\\~\\
{=}
\begin{bmatrix}
1\times4+9\times(-5) & 1\times2+9\times(-2)\\
3\times4+(-12)\times(-5) & 3\times2+(-12)\times(-2)
\end{bmatrix}
\\~\\
{=}
\begin{bmatrix}
-41 & -16\\
72 & 30
\end{bmatrix}
$$

Where each entry in the resulting matrix "c" is the sum of each entry in a's i'th row multiplied by b's j'th row:

$$
c_{ij}=
\sum_{k=1}^n a_{ik}b_{kj}
$$

Matrix is a wide topic, and you can learn about it for years, but I hope you now have a very very basic understanding of the structure, operations, and importance of matrices.

## What is a Tensor

Next, let's talk about tensors. A tensor is just a value. More specifically, it is a collection of an infinite number of values. This collection is so cool that it can contain any number whether it's a real number $R$ or an imaginary number $i$.
It is usually represented by a matrix.
$$
\begin{bmatrix}
4 & -9\\
6 & 13\\
\end{bmatrix}
$$
$$
\begin{bmatrix}
4 & -9 & i & \frac{3\pi}{4} & -281.5\overline{3} & ...
\end{bmatrix}
$$

## Manifold

Moving on to manifolds. A manifold is a space. Our basic manifold that we think of is the 2d Euclidean space where every value and object exsists in a flat and straight 2d grid where the horizontal axis is perpendicular to the vertical axis.
A value exists in every single point in that manifold. All values are tensors.
A manifold can be relative which means there can be many perspectives just like how you can have your perspective and a person in intersteller space can have their perspective.

## Differencial Manifold And Integration

When a manifold is differentiated, it is being "cut" into many infinitely small flat Euclidean spaces.
If you are learning or have learned calculus, please pay attention to this part because this will sound familiar. Imagine there is a curved line like: 
$$f(x)=x^3$$
When you differentiate it, you will cut it into an infinite number of thin rectangles. The result you get is
$$f'(x)=3x^2$$
 
We can also integrate curves by combining those infinitely thin rectangles.

$$g(x)=\int_{a}^b 3x^2\space dx=x^3+c$$
Since integration and differentiation are usually assymetric as integration introduces a new constant $c$, you may worry that when differentiating and then integrating a manifold, data may get lost or modified in the process. However, since the constant $c$ in the function $g$ only shifts the function $f$ up and down, it represents the same thing if you move your perspective up and down by that constant $c$. 

Imagine this process of differentiating a manifold as taking down a lego building and convert the building into individual blocks. In this analogy, each block represents an infinitely small Euclidean space. If you integrate this manifold, you are converting those blocks into a different building. But note that the new building consists of the same blocks as the old building.

## Pythagorean Theorem and the Law of Cosines

Before I talk about the exciting stuff, let's review the law of cosines.
Remember this?

$$a^2+b^2=c^2$$

Yeah, this is the famous pythagorean theorem. It is used to find the side lengths of right triangles. However, in this video, pythagorean theorem is too weak. We need a stronger theorem that also works with non-right triangles.
This is where the Law of Cosines shine. It does exactly that.

$$a^2 = b^2 + c^2 - 2bc\cos A$$

## Flatten a Planet

Ok, now that we've reviewed the famous Law of Cosines (or infamous if you hate math), we can finally get into the exciting part. Here, I generated a planet, I will call it planet 404 because I hate those stupid bugs in my code, so don't judge me. A cartographer called Euclid wants to map this planet, but he cannot find a way to completely and perfectly flatten the planet from a 3D sphere to a 2D plane. But, since me and Euclid are competitors, I secretly know a good way to create an approximated map just like the world map of our Earth (oh and please don't tell him that, it's a top secret).

### Longitude and Latitude

On this planet, I used a UV-Sphere mesh mapping, which means that the mesh consists of quads cut by the longitudinal and latitudinal lines. Btw, in case you don't know, latitudinal lines are horizontal and longitudinal lines are vertical.

Now that we defined our lines, we can see that every adjacent longitudinal lines forms a quad with every adjacent latitudinal line, well except the poles. The shapes on the poles are triangles but we can just say that one of the quad's points overlaps with another. Each quad represents a Metric Tensor, which I will tell you all about in a few seconds, but first let's see how we can transform this planet to a flat surface, or as physicists like to say, transform the planet from the current curved manifold to a flat manifold.

Now, you might be wondering, a sphere has a curved surface, so these quads are not truly flat. Remember when I talked about differenciable manifolds? If we use calculus to differentiate this manifold into infinitely small flat quads, we can construct this sphere with those flat quads just like when we can construct a curve by integrating infinitely thin rectangles.

Ok, next, we would take each quad, then move each piece to their corresponding location so that they are all lying next to each other. Then, we rotate each part so that their normals point towards us. We can observe that this shape is a rough map of the planet. But, we can see that there are holes on this new map, and I don't think google maps has holes every few square kilometers. We can solve this issue by first stretching the quad in the x axis and y axis. Then we skew the quads so that they fill in the holes. Unfortunately, I don't have enough time to code this in my 3d simulation program, so just use your flourishing imagination that vertices of the quads are stretched and rotated to meet their neighboring quads, forming a map of planet 404 that's like the world map of the Earth. By the way, to do the skewing, you need to use the law of cosines because the quads do not have $90\degree$ angles.

We are finally done creating a map of this planet. The process we just did is a simple example of transforming differencial manifolds using metric tensors.

### At Long Last, Tell Me About The Metric Tensor

So, what is the the metric tensor? Just like I said, each individual quad in this example has a metric tensor, and each metric tensor is a matrix that contains values of the amount its corresponding quad stretched in the x and y direction. We also skewed each quad by some angle, so, there is a final value here that represents the amount skewed. If you are observent, you might notice that there is a fourth element in the bottom left, that is essentially the same as the element in the top right, but it represents how much the quad skewed from the y axis to the x axis instead of how much the quad skewed from the x axis to the y axis. Thus, this value is redundant in most calculations as it can be easily calculated using the top right value.
Alright, that's all the metric tensor is... or is it...

$$
\begin{bmatrix}
stretch_x & \theta_{xy} \\
\theta_{yx} & stretch_y
\end{bmatrix}
$$


## What is Metric Tensor in General Relativity

Yes, the example I showed with planet 404 *is* a metric tensor, but in relativity, the metric tensor is different. It has four stretch components instead of two, which represents how stretched the time, x, y, and z axis are. There are also six angle components representing how much each axis skewed with another axis.

$$
\begin{bmatrix}
1 & \theta_1 & \theta_2 & \theta_3\\
{...} & -1 & \theta_4 & \theta_5\\
{...} & {...} & -1 & \theta_6\\
{...} & {...} & {...} & -1
\end{bmatrix}
$$

## What is Metric Space

Now that we talked about the core of metric tensors, let's understand what the term "Metric Space" means. A Metric Space is a set with a metric. The metric defines the distance between any two members in the set. Usually, the set contains points, and the metric defines the distance between any two points in that set. The metric component of the metric space must include the following properties:

1. The distance between any two points is zero if the two points are the same point.
2. Distance is positive.
3. Distance from A to B is the same as distance from B to A.
4. For every point C, distance from A to B is always shorter than or equal to the distance from A to C to B. 

So, how is Metric Space conneted to Metric Tensor? Metric Tensors can only give distances in an infinitely small, microscopic flat spacetime, whereas Metric Space gives the distance between any two points regardless of how apart they are and how curved the manifold is.

## The Euclidean, Minkowski, and the Schwarzschild Metric

You are probably very familiar with the Euclidean Metric.

$$
\begin{bmatrix}
xx & 0 \\
0 & yy
\end{bmatrix}
$$

Notice the zeros in the matrix? They tell us that there is no angle/curvature to this point.
In this Metric, the distance between any two points is calculated using the pythagorean theorem of the decomposed components of lengths.

$$
L = \int_a^b\sqrt{(dx)^2+(dy)^2}
$$

***

The Minkowski Metric is also called the Flat Spacetime.

$$
\begin{bmatrix}
1 & 0 & 0 & 0\\
0 & -1 & 0 & 0\\
0 & 0 & -1 & 0\\
0 & 0 & 0 & -1
\end{bmatrix}
$$

It is used in Special Relativity and is the one I showed you a few minutes ago.
Those 1, -1, -1, -1 in the matrix represents the coefficients of this equation:
$$
ds^2=c^2dt^2-dx^2-dy^2-dz^2
$$

Remember this hyperbola in Mr. Khalili's textbook? This is an application of the Minkowski Metric. This ensures that the spacetime intervals in a flat spacetime are independent of the inertial frames of references they are recorded in. The equation of a hyperbola is used to calculate the "straight" distance between any two points in the spacetime cone.
(Show cone demo)
Let me emphasize this again, this only works with flat spacetime. You can use the Minkowski Metric in a curved spacetime, but you have to integrate infinitely small spacetime cones with Minkowski Metric to approach the curved spacetime.

***

The Schwarzschild Metric is used in general relativity, and it is used to describe the spacetime around spherical objects like planets, stars, and even blackholes. It only works if the singularity has no charge and does not spin. In this metric, all blackholes are the same except their mass.  In this matrix, the Schwarzschild radius $r_s$ is the radius of which the event horizon of blackholes exist, and can be measured using the Schwarzschild Metric. By using this metric, we can calculate cool things like how small the sun needs to be for it to turn into a singularity (if the sun does not spin and has no charge), which is when its radius shrinks from its current 700,000 kilometers to about 3 kilometers. Thus, if the metric is describing the sun, $r_s$ would equal 3, and $r$ would equal 700,000.

$$
g_{\mu{v}}=
\begin{bmatrix}
(1-\frac{2GM}{rc^2}) & 0 & 0 & 0\\
0 & -(1-\frac{2GM}{rc^2})^{-1} & 0 & 0\\
0 & 0 & -r^2 & 0\\
0 & 0 & 0 & -r^2sin^2\theta
\end{bmatrix}
$$

$$
g_{\mu{v}}=
\begin{bmatrix}
(1-\frac{r_s}{r}) & 0 & 0 & 0\\
0 & \frac{1}{-(1-\frac{r_S}{r})} & 0 & 0\\
0 & 0 & -r^2 & 0\\
0 & 0 & 0 & -r^2sin^2\theta
\end{bmatrix}
$$

If you studied calculus before, you may observe that as $r$ goes to infinity, this metric becomes a Minkowski metric.

This is every you need to know about metrics in general relativity. Hopefully you enjoyed this video and learned something new today. Thank's for watching!

## Citations
1. [What is the relationship between a metric tensor and a metric? - Mathematics Stack Exchange](https://math.stackexchange.com/questions/2856754/what-is-the-relationship-between-a-metric-tensor-and-a-metric#:~:text=In%20short%3A,between%20(infinitesimally)%20close%20points.)
2. 
[^1]:This is not the only matrix multiplication operation.
