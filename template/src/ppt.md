---
marp: true
style: @import url('https://unpkg.com/tailwindcss@^2/dist/utilities.min.css');
---


![bg vertical](./img/final_cover.jpg)


---

# Code

```cpp
// concept
template <typename T, typename... Args>
concept is_valid_ctor = requires(Args&&... args) {
  { T(std::forward<Args>(args)...) };
};

// constraint by is_valid_ctor
template <typename T, typename ...Args>
auto kazen_malloc(Args&&... args) requires is_valid_ctor<T, Args...> {
  return new T(std::forward<Args>(args)...);
}
```


---

$$I_{xx}=\int\int_Ry^2f(x,y)\cdot{}dydx$$

---

# Multi columns in Marp slide

<div class="grid grid-cols-2 gap-4">
<div>


## 代码实现
```cpp
template <typename T, typename... Args>
concept is_valid_ctor = requires(Args&&... args) {
  { T(std::forward<Args>(args)...) };
};

template <typename T, typename ...Args>
auto kazen_malloc(Args&&... args) requires is_valid_ctor<T, Args...> {
  return new T(std::forward<Args>(args)...);
}

```

</div>
<div>

## 代码解释

Tempore ad exercitationem `necessitatibus` nulla, optio distinctio illo non similique? Laborum dolor odio, ipsam incidunt corrupti quia nemo quo exercitationem adipisci quidem nesciunt deserunt repellendus inventore deleniti reprehenderit at earum.

</div>
</div>

