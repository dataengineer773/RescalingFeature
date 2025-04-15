We need to rescale the values of a numerical feature to be between two values, Use scikit-learn’s MinMaxScaler to rescale a feature array, Rescaling is a common preprocessing task in machine learning. Many of the algorithms described later
in this book will assume all features are on the same scale, typically 0 to 1 or –1 to 1. There are a
number of rescaling techniques, but one of the simplest is called min-max scaling. Min-max scaling
uses the minimum and maximum values of a feature to rescale values to within a range. Specifically,
min-max calculates, where x is the feature vector, xi
is an individual element of feature x, and x’
i
is the rescaled element. In
our example, we can see from the outputted array that the feature has been successfully rescaled to
between 0 and 1, scikit-learn’s MinMaxScaler offers two options to rescale a feature. One option is to use fit to calculate
the minimum and maximum values of the feature, then use transform to rescale the feature. The
second option is to use fit_transform to do both operations at once. There is no mathematical
difference between the two options, but there is sometimes a practical benefit to keeping the operations
separate because it allows us to apply the same transformation to different sets of the data.
