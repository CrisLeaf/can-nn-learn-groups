# Can a Neural Network Learn an Algebraic Object?

Yes. It even does so with excellent results.

Here we test the capacity of a neural network (a simple one) to learn an algebraic object. The group structure. Specifically the S_6 permutations.

A group structure is a subset of S_6 that satisfies 4 specific properties:

- Closure.
- Identity.
- Inverses.
- Associativity.

More information can be found on: [working...](http://www.google.cl/)

## Requirements

The Python Notebook was written using a Python 3.9 environment, and the following libraries:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [Matplotlib](http://matplotlib.org/)
- [Scikit-Learn](http://scikit-learn.org/stable/)
- [TensorFlow](https://www.tensorflow.org/)

And to see the graph of a neural network you will need:
- [Pydot](https://pypi.org/project/pydot/)
- [Graphviz](https://graphviz.gitlab.io/download/)


## Dataset

The dataset was created using an script (not included). 

For the positive target, the program randomly select a subset of S_6 and then add everything that's missing until the 4 properties are reached. For the negative target, we just randomly selected subsets and assumed they were not groups.

Note that the subsets with a group structure are insanely rare. So randomly selecting some subset will result in a negative case with a 99.99...%, where the three points denote more than two hundred 9's.


## Results

The neural network can learn the group structure with an incredible score.


## Things to be done

- [X] Check if a neural network can learn a group estructure without considering the identity condition. (omiting the identity column)
- [ ] Create a blog where the algebraic part is explained.
- [ ] Use 1 million negative cases vs ~1000 positive cases. (A ratio of 1/1000)


## Support

Give a :star: if you like it :hugs:.