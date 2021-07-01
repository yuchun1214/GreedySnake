# Greedy Snake

## Coding convention

* language : C
* struct 
    * type : list_element_t
    ```c=
    struct list_element_t{
        struct list_element_t * next;
        struct list_element_t * prev;
    };
    typedef struct list_element_t list_element_t;
    ```
    * field : private variables should start with underline
* function : isFoo
    * private function should be implemented in .c file
    * public function should be defined in .h file and be implemented in .c file
    ```c=
    bool isFoo();
    ```
* variable : list_element
* const : all capital
* object-like macro : all capital
* function-like macro : similar to function

## Data structure

```c=
typedef struct array_t array_t;
struct array_t{
    int size;
    void * _array;
    int _capacity;
};
```

```c=
#define tos(array_t *, type)
#define push(array_t *, type, var)
#define pop(array_t *)
#define resize(array_t *, type)
#define initialize(array_t *, type)
```

## Reference

[ncurses](https://invisible-island.net/ncurses/ncurses.html)