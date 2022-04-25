# Transformer-based-NER-for-Indian-languages
This repository contains different transformer based Deep learning models for NER task in Indian languages.

Step 1: Preprocessing
      
      run preproccessing.py with below command line arguments.
      Path of three data files: train, valid and test 
      
 Step 2:Training
        
        run train.py with  below command line arguments.
        model_version, train_data-file, model_max_length, number_of_epochs, batch_size, learning_rate
        
 
 Step 3:Evaluation
        
        a.run eval_valid.py for evaluation on valid data with  below command line arguments.
        model_version, valid_data_file, model_max_length, number_of_epoch, batch_size
 
        b.  run eval_test.py for evaluation on test data with  below command line arguments.
        model_version, best_model_path, test_data_file, model_max_length,  batch_size
        
        best_model_path = Training saves model for each epoch. Select model which gives highest F1-score on valid_data.



model_version =  'ai4bharat/indic-bert' / 
                 'xlm-roberta-base' / 
                 'xlm-roberta-large' / 
                 'google/muril-large-cased' /
                 'google/muril-base-cased' / 
                 'bert-base-multilingual-cased'
