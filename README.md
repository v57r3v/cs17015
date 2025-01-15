java c
Optimization   and   Algorithms 
February 6,   2023 
Exam
1. Deconﬁicted      trajectories.       A   trajectory   T   of   duration   T   in Rd         is   a   sequence   of   T points   in Rd, denoted   as   T   = {x(1),   x(2), . . . ,   x(T)}, with   x(t) ∈ Rd      for   1 ≤ t   ≤ T.   Note that t   denotes discrete-time; thus t   is an integer   (such as   t   = 0, 1,   2,   3. . . .).Let   T1      =   {x1   (1),   x1   (2), . . . ,   x1   (T)}   and   T2      =   {x2   (1),   x2   (2), .   .   .   ,   x2   (T)}   be   two   tra-   jectories   of   duration   T   in Rd.      We   say   that   T1       and   T2       are   space-decon丑icted   if   Ⅱx1   (t) - x2   (s)Ⅱ2      >   ∈   for   1   ≤   t,   s   ≤   T,   where   ∈   is   a   given   positive   number.   We   say   that T1    and   T2      are time-decon丑icted   if   Ⅱx1   (t) - x2   (t)Ⅱ2    >   ∈   for   1   ≤ t   ≤   T.Consider the following two controlled   dynamic linear   systems.   The   state   of system
1 at time t   is denoted by x1   (t) ∈ Rd   ,   for   1   ≤   t   ≤   T   and   obeys   the   recursion
x1   (t + 1) =   A1x1   (t)   +   B1u1   (t),            0 ≤ t ≤ T - 1,where A1    ∈ Rd×d      and B1      ∈ Rd×p      are   given   matrices,   x1   (0)   ∈ Rd      is   a   given   initial   state and u1   (t) ∈ Rp      is the   control   input   of   system   1   at   time   t,   for   0   ≤   t   ≤   T   -   1.   Note   that   the   trajectory   T1    depends   on   the   inputs   u1   (t), 0 ≤   t   ≤   T   -   1.
Similarly, for system 2   we   have
x2   (t + 1) =   A2x2   (t)   +   B2u2   (t),            0 ≤ t ≤   T - 1.
Note   that   the   trajectory   T2    depends   on   the   inputs   u2   (t), 0 ≤   t   ≤   T   -   1.
Finally,   let   Tref         =   {r(1),   r(2), . . . ,   r(T)}   be   a   given,   ﬁxed   reference   trajectory   of duration T   in Rd.
We   want   to   design   the   control   inputs   u1   (t) (0 ≤ t   ≤ T   -   1) and   u2   (t) (0 ≤ t   ≤ T   -   1)   so   that:
•   the ﬁnal state x1   (T) of system 1 is as close as possible to a given, desired state   p1      ∈ Rd;
•   the ﬁnal state x2   (T) of system 2 is as close as possible to a given, desired state   p2      ∈ Rd;
•   the trajectories T1    and T2      are   time-deconflicted;
•   the trajectories T1    and Tref      are   space-deconflicted;
•   the trajectories T2    and Tref      are   space-deconflicted.
One of the following problem formulations is suitable for the given context.

Which one?
Write your answer (A, B, C, D, E, or F) in the box at the top of page 1 
2. Unconstrained   optimization.    Consider   the optimization problem

The point x★ = 0 is a global minimizer of   (7) for   one   of the following   choices   of a:
(A)   a = -2
(B)   a = -1
(C)   a   =   0
(D)   a   = 1
(E)   a = 2
(F)   a =   3
Which one?
Write your answer (A, B, C, D, E, or F) in the box at the top of page 1 
Hint:    the numerical values log(2) ≈ 0.7 and   log(3) 代 写Optimization and Algorithms 2023 ExamJava
代做程序编程语言≈   1.1   might   be   useful
3. Gradient      descent      algorithm.       Consider   the   function   f   : R2      → R given   by   f   (a,   b)   = 2/1a2+(a−b)2. Suppose we do one iteration of the gradient descent algorithm (applied to f) starting from the point

and using the   stepsize   1.
Which   of   the   following   points   is   the   next   iteration   x1   ?
Write your answer (A, B, C, D, E, or F) in the box at the top of page 1 
4. Signal-denoising    as      a    least-squares      problem.          Consider   the   function   f : Rn         → R,   f   (r)   =   rT   Dr,   where   D   is   a   given   n   × n   diagonal   matrix   with   positive   diagonal entries:

with di    >   0   for   1   ≤   i   ≤   n.
Consider the following optimization problem
where the variables to optimize are   s   ∈ Rp      and   v   ∈ Rn;   the   matrix   A   ∈ Rn×p      and   the   vectors   y   ∈ Rn   ,   and   s   ∈ Rp      are   given.    This   problem   can   be   interpreted   as   a   signal-denoising   problem:   we   observe   y   and want to   decompose   it   as the   sum   of a   signal of   interest s and noise v; we know that s should be close to the nominal signal   s   and   that   v   should   be   close   to   zero   (the   larger   the   di,   the   more   conﬁdent   we   are   that the component vi    should be   close   to   zero).
Problem   (8) can be reduced to   a   least-squares   problem   involving   only   the   variable   s, that is, it can be reduced   to   a   problem   of the form.	

for some matrix A   and vector   β   .
Give   A   and   β   in   terms   of   the   constants   D   , y   , A,   and   s.
5. A   simple   optimization   problem.    Consider   the   function   f   : R2    → R, f(x) = 2/1xTMx,
where

The constants a   and   b   satisfy   0 < a < b.
Solve in closed-form. the optimization problem
where 1 denotes the vector 1 = (1, 1). 
6. A    convex    optimization   problem.    Consider the following optimization problemwhere   the   variables   to   optimize   are   xi      ∈ R,   for   1   ≤   i   ≤   n.    The   vectors   a   i      ∈ Rp   ,   1   ≤   i   ≤   n   and   b   ∈ Rp    are given.    The constants   ci,   1   ≤   i   ≤   n,   are also   given.    The   function g : R → R is deﬁned as follows:

Show that   (11) is a convex optimization problem.
7. A      convex   function    based    on      a      worst-case      representation.          Show   that   the   function   f   : R → R,f   (x) = max   {Ⅱ(a + u)x — bⅡ2      :    ⅡuⅡ2   = r}                                                                              (12)
is convex, where the vectors a,   b   ∈ Rn      and the   constant   r   >   0   are   given.
In words:    f   takes   as   input   a   number   x   and returns   as output the   largest   value   of   the expression
Ⅱ(a + u)x   —   bⅡ2
as u   ranges over the sphere centered at the   origin   and with   radius   r.

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
