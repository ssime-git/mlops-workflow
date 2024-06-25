# Wine Quality

MLOps project to predict the quality of a wine given certain parameters.

Workflow: 
1. Update the config.yaml with the necessary directories for each step.
The steps to be followed are: data ingestion, data validation, data processing, model training and model evaluation.
2. Update params.yaml with the hyperparameters of the model.
3. Update schema.yaml with the informatic type of variables.
4. On common utils we will have functions used more than once (namely read_yaml, create directories and save_json).
5. On entity.py we'll have the configuration of the different class objects we'll be using, namely DataIngestion, DataValidation, DataTransformation, ModelTrainer and ModelEvaluation.
6. Our config_manager.py will help us read the paths from the config.yaml file as well as the model hyperparameters and pass them on to the class objects. If needed, it will create the necessary folders through the create_directories function present in the common_utils.py file.
7. On data and models we'll create the necessary scripts for each step: data ingestion, data validation, data transformation, model training and model evaluation.
8. Create the pipeline step by step.