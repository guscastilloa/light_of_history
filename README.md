# Light of History: Historical Event Classification

This repository contains code for training and deploying a binary classifier to identify historical events in Wikipedia articles. The project uses DistilBERT to classify text as either "historical event" or "not historical event," achieving validation accuracy above 99.5%.

## Project Components

- Training pipeline using DistilBERT for binary classification
- Wikipedia article processing and classification system
- Validation and testing frameworks
- Batch processing capabilities for large-scale classification

## Technical Details

- Model: DistilBERT with binary classification head
- Training Data: 211,525 balanced examples
- Split: 80/20 train/validation
- Hardware: Google Colab with NVIDIA T4 GPU
- Implementation: TensorFlow/Hugging Face Transformers

## Resources

- Training dataset available on HuggingFace: [guscastilloa/dbpedia_historical_events](https://huggingface.co/datasets/guscastilloa/dbpedia_historical_events)
- Model weights and classification outputs archived on Zenodo: [doi:10.5281/zenodo.14126493](https://doi.org/10.5281/zenodo.14126493)

## Key Features

- High-accuracy binary classification (>99.5% validation accuracy)
- Efficient processing of large text datasets
- Probability scores for classification decisions
- Edge case handling for ambiguous historical events

## Future Development

- Implementation of k-fold and time-based cross-validation
- Scaling to full Wikipedia dataset (9M+ articles)
- Enhanced error analysis
- Integration of human-validated data

## Citation

If you use this code in your research, please cite our Zenodo archive:
```bibtex
@dataset{castillo_2024_14126493,
  author       = {Castillo Alvarez, G. A. and
                  Garcia-Figal, A. and
                  Lage-Castellanos, A. and
                  Baez-Silva, A. M.},
  title        = {{Light of History: Model weights and classified output}},
  month        = nov,
  year         = 2024,
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.14126493},
  url          = {https://doi.org/10.5281/zenodo.14126493}
}
```
