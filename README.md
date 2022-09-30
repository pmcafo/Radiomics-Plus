# Radiomics Plus\nThis collection of scripts is designed to perform Radiomics on three-dimensional medical images (like PET and CT). They can also classify a wide range of image types, both 2D and 3D, using classic texture analysis methods (e.g., GLCM).\n\nThe script "batch.py" leverages PyRadiomics packages to extract features from images, including first order and texture features. These features can aid in further image classification. You can even customize the feature extraction settings as per your needs. More information can be found on the PyRadiomics website: https://pyradiomics.readthedocs.io/en/latest/.\n\nThe script "change_matlab_to_python.py" converts images from matlab-format to nrrd-files for use in "batch.py".\n\n"functions.py" contains all feature selection and classification methods, which are imported into "classification.py".\n\nThe "classification.py" script classifies images using the feature selection methods and classification methods defined in "functions.py", testing accuracy with a nested cross validation. Here you can also test the effect of using different amou