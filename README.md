# Auto_machine_learning
A code to to prediction on machine learning problem without any human intervention

The folder lib contains all the necessary function of the library

data_converter.py performs various data conversions for the ChaLearn AutoML challenge (No modification from the initial baseline of the challenge)

data_io performs various input/output opeartions for the ChaLearn AutoML challenge (No modification from the initial baseline)

data_manager.py various input/output opeartions for the ChaLearn AutoML challenge (No modification from the initial baseline)

models.py Rough sketch of a class that "solves" the AutoML problem. We illustrate various type of data that will be encountered in the challenge can be handled.
         Also, we make sure that the model regularly outputs predictions on validation and test data, such that, if the execution of the program is interrupted (timeout)
         there are still results provided by the program.
         We use ensemble methods with some few modification for different configurations where the number of samples is small in comparison to the number of features for example
         that vote on an increasing number of classifiers. For efficiency, we use WARM START that re-uses
         already trained base predictors, when available.
