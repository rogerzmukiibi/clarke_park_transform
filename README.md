# Clarke and Park Transforms

## Clarke Transform
> "In electrical engineering, the alpha-beta (α-β-γ)transformation, also known as the Clarke transform, is a mathematical transformation applied to simplify the analysis of three-phase circuits. Conceptually, it is similar to the dq0 transform. A very useful application of the alpha-beta transform is the generation of a reference signal used for [space vector modulation control](https://en.wikipedia.org/wiki/Space_vector_modulation)."<br/>
[Wikipedia](https://en.wikipedia.org/wiki/Alpha%E2%80%93beta_transformation)

The Clarke Transform consists of a system where the alpha axis is completely aligned with phase A and the beta axis is in quadrature (90°) with it. This produces two sinusoidal curves shifted by 90 degrees. When the three-phase system is balanced, these alpha-beta curves have equal magnitude. When the system becomes unbalanced, their magnitudes differ.

![](https://www.mathworks.com/help/sps/ref/clarke_transform_model_scope_01.png) <br/>
(Source: [Mathworks](https://www.mathworks.com/help/physmod/sps/ref/clarketransform.html))

## Park Transform

> "The direct-quadrature-zero (dq0) transformation is a tensor that rotates the reference axis of a three-element vector system or a three-by-three matrix in order to simplify analysis. The dq0 transform is the product of the Clarke and Park transforms, first proposed by Robert H. Park in 1929." <br/>
[Wikipedia](https://en.wikipedia.org/wiki/Direct-quadrature-zero_transformation)

![](https://www.mathworks.com/help/sps/ref/park_transform_axes_01.png) ![](https://www.mathworks.com/help/sps/ref/park_transform_axes_02.png) <br/>
(Source: [MathWorks](https://www.mathworks.com/help/physmod/sps/ref/parktransform.html))

When applied to a balanced three-phase system, the Park transform produces constant values for d, q, and zero components. When an imbalance occurs, these values begin to oscillate (at twice the frequency of the original system).

When calculating the Park transform, we can align either the d-axis or the q-axis with phase A of the three-phase system. In this project, the d-axis was chosen for alignment with phase A, resulting in a graph similar to the one shown below.

![grafico resultante](https://www.mathworks.com/help/sps/ref/park_transform_q_model_scope_01.png)<br/>
(fonte: [MathWorks](https://www.mathworks.com/help/physmod/sps/ref/parktransform.html))

# How to Use This Software

The graphical interface of this program was designed to make usage as simple as possible. Therefore, this explanation will be brief. The steps for a typical execution are:
1. Run the file main.py. As the name suggests, it is the main file of the program and executes all instructions. When run correctly, a window will open;

2. In the opened window, you can input all program data. ***Note that the program will not generate graphs until all fields are properly filled;***

3. Units are displayed next to the fields, except for the "unit" and "Faults" fields, which are dropdown menus with predefined options;

4. Text fields, such as "frequency [Hz]:", accept only numbers, the decimal point ".", and the negative sign "-" to prevent possible errors that could disrupt code execution;

5. There is no specific order in which the data must be filled;

6. Once all fields are completed, simply click the "Calculate" button to generate the graphs based on the configured conditions;

7. A new window will then open to display the graphs. This window is interactive, allowing you to resize, zoom in/out, and analyze specific intervals;

8. To save the graphs, click the disk icon in the graph window and choose the file format and location. ***Note that the program does not automatically save these files!;***

9. If you want to generate new graphs, repeat steps 2 through 6. ***Note that previously generated graphs will be overwritten, so if you want to keep them, make sure to complete step 8!.***