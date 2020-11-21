# Google IME Handwriting Request

Example of direct usage of the API behind handwriting in google translate.

https://h7x4abk3g.github.io/google-ime-handwriting-request/

### Example request data:

```json
{
  "app_version": 0.4,
  "api_level": "537.36",
  "device": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 Edge/12.246",
  "input_type": 0,
  "options": "enable_pre_space",
  "requests": [
    {
      "writing_guide": {
        "writing_area_width": 500,
        "writing_area_height": 500
      },
      "pre_context": "",
      "max_num_results": 10,
      "max_completions": 0,
      "language": "ja",
      "ink": [
        [
          [139,204,288],
          [169,173,173],
          [27,51,75]
        ],
        [
          [213,213,216,219,221],
          [110,124,160,203,229],
          [57,81,105,129,153]
        ]
      ]
    }
  ]
}
```

where ink is an array of strokes. A stroke is formatted as an array containing three arrays. They contain every points x-values, y-values and the time between point creation and the beginning of the stroke.