# Caching System README

This README file provides an overview of the caching systems implemented using different algorithms.

## Task 0: Basic dictionary - BasicCache

```python
class BasicCache(BaseCaching):
    """
    Caching system without any limit.
    Inherits from BaseCaching and uses a dictionary as cache_data.
    """

    def put(self, key, item):
        """
        Assigns the item value for the key key in the cache_data dictionary.
        If key or item is None, this method does nothing.
        """
        # Add your implementation here

    def get(self, key):
        """
        Returns the value in cache_data linked to key.
        If key is None or if the key doesn't exist in cache_data, return None.
        """
        # Add your implementation here
```

## Task 1: FIFO caching - FIFOCache

```python
class FIFOCache(BaseCaching):
    """
    Caching system that uses First-In-First-Out (FIFO) algorithm.
    Inherits from BaseCaching and uses a dictionary as cache_data.
    """

    def __init__(self):
        super().__init__()

    def put(self, key, item):
        """
        Assigns the item value for the key key in the cache_data dictionary.
        If key or item is None, this method does nothing.
        If the number of items in cache_data is higher than BaseCaching.MAX_ITEMS,
        the first item put in cache (FIFO algorithm) is discarded and printed as DISCARD.
        """
        # Add your implementation here

    def get(self, key):
        """
        Returns the value in cache_data linked to key.
        If key is None or if the key doesn't exist in cache_data, return None.
        """
        # Add your implementation here
```

## Task 2: LIFO Caching - LIFOCache

```python
class LIFOCache(BaseCaching):
    """
    Caching system that uses Last-In-First-Out (LIFO) algorithm.
    Inherits from BaseCaching and uses a dictionary as cache_data.
    """

    def __init__(self):
        super().__init__()

    def put(self, key, item):
        """
        Assigns the item value for the key key in the cache_data dictionary.
        If key or item is None, this method does nothing.
        If the number of items in cache_data is higher than BaseCaching.MAX_ITEMS,
        the last item put in cache (LIFO algorithm) is discarded and printed as DISCARD.
        """
        # Add your implementation here

    def get(self, key):
        """
        Returns the value in cache_data linked to key.
        If key is None or if the key doesn't exist in cache_data, return None.
        """
        # Add your implementation here
```

## Task 3: LRU Caching - LRUCache

```python
class LRUCache(BaseCaching):
    """
    Caching system that uses Least Recently Used (LRU) algorithm.
    Inherits from BaseCaching and uses a dictionary as cache_data.
    """

    def __init__(self):
        super().__init__()

    def put(self, key, item):
        """
        Assigns the item value for the key key in the cache_data dictionary.
        If key or item is None, this method does nothing.
        If the number of items in cache_data is higher than BaseCaching.MAX_ITEMS,
        the least recently used item (LRU algorithm) is discarded and printed as DISCARD.
        """
        # Add your implementation here

    def get(self, key):
        """
        Returns the value in cache_data linked to key.
        If key is None or if the key doesn't exist in cache_data, return None.
        """
        # Add your implementation here
```

## Task 4: MRU Caching - MRUCache

```python
class MRUCache(BaseCaching):
    """
    Caching system that uses Most Recently Used (MRU) algorithm.
    Inherits from BaseCaching and uses a dictionary as cache_data.
    """

    def __init__(self):
        super().__init__()

    def put(self, key, item):
        """
        Assigns the item value for the key key in the cache_data dictionary.
        If key or item is None, this method does nothing.
        If the number of items in cache_data is higher than BaseCaching.MAX_ITEMS,
        the most recently used item (MRU algorithm) is discarded and printed as DISCARD.
        """
        # Add your implementation here

    def get(self, key):
        """
        Returns the value in cache_data linked to key.
        If key is None or if the key doesn't exist in cache_data, return None.
        """
        # Add your implementation here
```

## Task 5: LFU Caching - LFUCache

```python
class LFUCache(BaseCaching):
    """
    Caching system that uses Least Frequency Used (LFU) algorithm.
    Inherits from BaseCaching

 and uses a dictionary as cache_data.
    """

    def __init__(self):
        super().__init__()

    def put(self, key, item):
        """
        Assigns the item value for the key key in the cache_data dictionary.
        If key or item is None, this method does nothing.
        If the number of items in cache_data is higher than BaseCaching.MAX_ITEMS,
        the least frequency used item (LFU algorithm) is discarded and printed as DISCARD.
        If there are multiple items with the same least frequency, the LRU algorithm is used to discard the least recently used.
        """
        # Add your implementation here

    def get(self, key):
        """
        Returns the value in cache_data linked to key.
        If key is None or if the key doesn't exist in cache_data, return None.
        """
        # Add your implementation here
```
