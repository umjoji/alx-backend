# Pagination README

This README file provides an overview of the functions included in this project for pagination and hypermedia pagination of a dataset.

## Task 0: Simple helper function - index_range

```python
def index_range(page: int, page_size: int) -> tuple:
    """
    Return a tuple of size two containing a start index and an end index
    corresponding to the range of indexes to return in a list for the given pagination parameters.
    """
    # Add your implementation here
```

## Task 1: Simple pagination - get_page

```python
def get_page(page: int = 1, page_size: int = 10) -> List[List[str]]:
    """
    Return the appropriate page of the dataset (i.e. the correct list of rows) based on the given page and page_size.
    If the input arguments are out of range for the dataset, an empty list should be returned.
    """
    # Add your implementation here
```

## Task 2: Hypermedia pagination - get_hyper

```python
def get_hyper(page: int = 1, page_size: int = 10) -> Dict[str, Union[int, List[List[str]], None]]:
    """
    Return a dictionary containing pagination information for the dataset.
    The dictionary will include keys for page_size, page, data, next_page, prev_page, and total_pages.
    """
    # Add your implementation here
```

## Task 3: Deletion-resilient hypermedia pagination - get_hyper_index

```python
def get_hyper_index(index: Optional[int] = None, page_size: int = 10) -> Dict[str, Union[int, List[List[str]]]]:
    """
    Return a dictionary containing pagination information for the dataset based on the given index and page_size.
    The dictionary will include keys for index, next_index, page_size, and data.
    """
    # Add your implementation here
```
