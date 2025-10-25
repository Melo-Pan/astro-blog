# AstroPaper 📄

![AstroPaper](public/astropaper-og.jpg)
![Typescript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![GitHub](https://img.shields.io/github/license/satnaing/astro-paper?color=%232F3741&style=for-the-badge)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white&style=for-the-badge)](https://conventionalcommits.org)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg?style=for-the-badge)](http://commitizen.github.io/cz-cli/)

AstroPaper is a minimal, responsive, accessible and SEO-friendly Astro blog theme. This theme is designed and crafted based on [my personal blog](https://satnaing.dev/blog).

This theme follows best practices and provides accessibility out of the box. Light and dark mode are supported by default. Moreover, additional color schemes can also be configured.

This theme is self-documented \_ which means articles/posts in this theme can also be considered as documentations. Read [the blog posts](https://astro-paper.pages.dev/posts/) or check [the README Documentation Section](#-documentation) for more info.

## 🔥 Features

- [x] type-safe markdown
- [x] super fast performance
- [x] accessible (Keyboard/VoiceOver)
- [x] responsive (mobile ~ desktops)
- [x] SEO-friendly
- [x] light & dark mode
- [x] fuzzy search
- [x] draft posts & pagination
- [x] sitemap & rss feed
- [x] followed best practices
- [x] highly customizable
- [x] dynamic OG image generation for blog posts [#15](https://github.com/satnaing/astro-paper/pull/15) ([Blog Post](https://astro-paper.pages.dev/posts/dynamic-og-image-generation-in-astropaper-blog-posts/))

_Note: I've tested screen-reader accessibility of AstroPaper using **VoiceOver** on Mac and **TalkBack** on Android. I couldn't test all other screen-readers out there. However, accessibility enhancements in AstroPaper should be working fine on others as well._

## ✅ Lighthouse Score

<p align="center">
  <a href="https://pagespeed.web.dev/report?url=https%3A%2F%2Fastro-paper.pages.dev%2F&form_factor=desktop">
    <img width="710" alt="AstroPaper Lighthouse Score" src="AstroPaper-lighthouse-score.svg">
  <a>
</p>

## 🚀 Project Structure

Inside of AstroPaper, you'll see the following folders and files:

```bash
/
├── public/
│   ├── assets/
│   │   └── logo.svg
│   │   └── logo.png
│   └── favicon.svg
│   └── astropaper-og.jpg
│   └── robots.txt
│   └── toggle-theme.js
├── src/
│   ├── assets/
│   │   └── socialIcons.ts
│   ├── components/
│   ├── content/
│   │   |  blog/
│   │   |    └── some-blog-posts.md
│   │   └── config.ts
│   ├── layouts/
│   └── pages/
│   └── styles/
│   └── utils/
│   └── config.ts
│   └── types.ts
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

Any static assets, like images, can be placed in the `public/` directory.

All blog posts are stored in `src/content/blog` directory.

## 📖 Documentation

Documentation can be read in two formats\_ _markdown_ & _blog post_.

- Configuration - [markdown](src/content/blog/how-to-configure-astropaper-theme.md) | [blog post](https://astro-paper.pages.dev/posts/how-to-configure-astropaper-theme/)
- Add Posts - [markdown](src/content/blog/adding-new-post.md) | [blog post](https://astro-paper.pages.dev/posts/adding-new-posts-in-astropaper-theme/)
- Customize Color Schemes - [markdown](src/content/blog/customizing-astropaper-theme-color-schemes.md) | [blog post](https://astro-paper.pages.dev/posts/customizing-astropaper-theme-color-schemes/)
- Predefined Color Schemes - [markdown](src/content/blog/predefined-color-schemes.md) | [blog post](https://astro-paper.pages.dev/posts/predefined-color-schemes/)

> For AstroPaper v1, check out [this branch](https://github.com/satnaing/astro-paper/tree/astro-paper-v1) and this [live URL](https://astro-paper-v1.astro-paper.pages.dev/)

## 💻 Tech Stack

**Main Framework** - [Astro](https://astro.build/)  
**Type Checking** - [TypeScript](https://www.typescriptlang.org/)  
**Component Framework** - [ReactJS](https://reactjs.org/)  
**Styling** - [TailwindCSS](https://tailwindcss.com/)  
**UI/UX** - [Figma](https://figma.com)  
**Fuzzy Search** - [FuseJS](https://fusejs.io/)  
**Icons** - [Boxicons](https://boxicons.com/) | [Tablers](https://tabler-icons.io/)  
**Code Formatting** - [Prettier](https://prettier.io/)  
**Deployment** - [Cloudflare Pages](https://pages.cloudflare.com/)  
**Illustration in About Page** - [https://freesvgillustration.com](https://freesvgillustration.com/)  
**Linting** - [ESLint](https://eslint.org)

## 👨🏻‍💻 Running Locally

The easiest way to run this project locally is to run the following command in your desired directory.

```bash
# npm 6.x
npm create astro@latest --template satnaing/astro-paper

# npm 7+, extra double-dash is needed:
npm create astro@latest -- --template satnaing/astro-paper

# yarn
yarn create astro --template satnaing/astro-paper
```

## Google Site Verification (optional)

You can easily add your [Google Site Verification HTML tag](https://support.google.com/webmasters/answer/9008080#meta_tag_verification&zippy=%2Chtml-tag) in AstroPaper using environment variable. This step is optional. If you don't add the following env variable, the google-site-verification tag won't appear in the html `<head>` section.

```bash
# in your environment variable file (.env)
PUBLIC_GOOGLE_SITE_VERIFICATION=your-google-site-verification-value
```

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

> **_Note!_** For `Docker` commands we must have it [installed](https://docs.docker.com/engine/install/) in your machine.

| Command                              | Action                                                                                                                           |
| :----------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| `npm install`                        | Installs dependencies                                                                                                            |
| `npm run dev`                        | Starts local dev server at `localhost:4321`                                                                                      |
| `npm run build`                      | Build your production site to `./dist/`                                                                                          |
| `npm run preview`                    | Preview your build locally, before deploying                                                                                     |
| `npm run format:check`               | Check code format with Prettier                                                                                                  |
| `npm run format`                     | Format codes with Prettier                                                                                                       |
| `npm run sync`                       | Generates TypeScript types for all Astro modules. [Learn more](https://docs.astro.build/en/reference/cli-reference/#astro-sync). |
| `npm run cz`                         | Commit code changes with commitizen                                                                                              |
| `npm run lint`                       | Lint with ESLint                                                                                                                 |
| `docker compose up -d`               | Run AstroPaper on docker, You can access with the same hostname and port informed on `dev` command.                              |
| `docker compose run app npm install` | You can run any command above into the docker container.                                                                         |

> **_Warning!_** Windows PowerShell users may need to install the [concurrently package](https://www.npmjs.com/package/concurrently) if they want to [run diagnostics](https://docs.astro.build/en/reference/cli-reference/#astro-check) during development (`astro check --watch & astro dev`). For more info, see [this issue](https://github.com/satnaing/astro-paper/issues/113).

## ✨ Feedback & Suggestions

If you have any suggestions/feedback, you can contact me via [my email](mailto:contact@satnaing.dev). Alternatively, feel free to open an issue if you find bugs or want to request new features.

## 📜 License

Licensed under the MIT License, Copyright © 2023

---

Made with 🤍 by [Sat Naing](https://satnaing.dev) 👨🏻‍💻 and [contributors](https://github.com/satnaing/astro-paper/graphs/contributors).


# 位运算核心笔记

## 一、基础位运算符

| 运算符   | 名称        | C++ 符号 | 说明                             |
| :------- | :---------- | :------- | :------------------------------- |
| 按位与   | AND         | `&`      | 两位都为 1 时，结果为 1          |
| 按位或   | OR          | `\|`     | 任意一位为 1 时，结果为 1        |
| 按位异或 | XOR         | `^`      | 两位不同时，结果为 1             |
| 按位取反 | NOT         | `~`      | 逐位取反，0 变 1，1 变 0         |
| 左移     | Left Shift  | `<<`     | 所有位向左移动，右侧补 0         |
| 右移     | Right Shift | `>>`     | 所有位向右移动，左侧补符号位或 0 |

## 二、二进制状态压缩 (状压)

**核心思想**：将一个长度为 `n` 的布尔数组（或任何具有两种状态的元素集合）压缩到一个整数中。整数的每一位对应一个元素的状态。这本质上是**从描述到编码**的思维转变。

#### 核心作用

1.  **状态的索引化**
    *   **痛点**：在 DP 中，无法直接创建 `dp[vector<bool>]` 这样的数据结构。使用 `map` 或 `unordered_map` 效率低下。
    *   **解决**：状压后的整数 `mask` 可直接用作数组下标 `dp[mask]`，实现 `O(1)` 存取。这极大提升了空间和时间效率（例如，存储 `k` 个状态只需 `k` 个整数，而非 `k*n` 的空间）。

2.  **集合运算的降维打击**
    *   将 `O(n)` 的集合操作转化为 `O(1)` 的位运算。
    *   **并集 (Union)**: `mask_a | Wmask_b`
    *   **交集 (Intersection)**: `mask_a & mask_b`
    *   **差集 (A - B)**: `mask_a & (~mask_b)`

3.  **状态的遍历**
    *   `for (int mask = 0; mask < (1 << n); ++mask)` 枚举即可遍历所有 `2^n` 种状态。

#### 局限性与适用场景

*   **指数级复杂度**：状压并未改变问题的指数级本质，算法复杂度通常为 `O(2^n * poly(n))`。
*   **位数限制**：`int` (32位) 或 `long long` (64位) 决定了 `n` 的上限。
*   **适用场景**：
    *   **数据规模小**：核心元素数量 `n` 通常 `≤ 20`。
    *   **涉及子集/排列**：问题状态与集合的子集、排列或组合有关。
    *   **需要记录状态**：需在算法中（尤其 DP）记录“哪些元素已被使用/访问”等信息。

#### 常用技巧

| 操作                | C++ 实现             |
| :------------------ | :------------------- |
| **获取**第 `k` 位   | `(n >> k) & 1`       |
| **获取**后 `k` 位   | `n & ((1 << k) - 1)` |
| 将第 `k` 位**置 1** | `n \| (1 << k)`      |
| 将第 `k` 位**置 0** | `n & (~(1 << k))`    |
| 将第 `k` 位**取反** | `n ^ (1 << k)`       |

## 三、Lowbit 运算

**核心思想**：`lowbit(n)` 用于获取非负整数 `n` 在二进制表示中，**最靠右的 '1' 所代表的数值**。

*   **实现**：`lowbit(n) = n & (~n + 1) = n & -n` (利用了计算机补码的特性)

#### 核心作用

1.  **树状数组 (Fenwick Tree) 的基石**
    *   `lowbit` 是树状数组的理论核心。节点 `C[i]` 所管辖的区间长度恰好是 `lowbit(i)`。
    *   **更新** `add(i)`: 通过 `i += lowbit(i)` 向上层传递。
    *   **查询** `query(i)`: 通过 `i -= lowbit(i)` 向前缀回溯。

2.  **高效遍历状态的所有 '1' 位**
    *   **常规方法**：`for` 循环 `n` 次，复杂度 `O(n)`。
    *   **`lowbit` 方法**：直接跳到下一个 '1'，复杂度为 `O(k)` (k 为 '1' 的个数)。当 `k << n` 时效率更高。

    ```cpp
    // 遍历 mask 中所有的 '1'
    while (mask > 0) {
        int lb = mask & -mask; // 找到最低位的 1
        // lb 是 2 的幂，可用于计算位置或直接使用
        // int pos = __builtin_ctz(lb); // GCC 内置函数，快速获取位置
      
        // ... 处理 lb ...

        mask -= lb; // 从 mask 中移除这个 '1'
    }
    ```

# 递推与递归核心笔记

## 一、核心思想：分解问题

递推（Iteration）和递归（Recursion）都是解决问题的两种基本方法，其核心思想一脉相承：**将一个复杂的大问题，分解为若干个规模更小、结构相同的子问题来求解。**

*   **递归 (Top-Down)**：从大问题出发，调用自身去解决更小的子问题，直到遇到无法再分解的**基本情况（Base Case）**，然后逐层返回结果。它更符合人类的直觉思维。
    *   **口诀**：先调用，后求解。

*   **递推 (Bottom-Up)**：从已知的**初始状态（Initial State）**出发，通过**递推关系式**，一步步计算出更大规模问题的解，直到目标问题。它通常以循环（`for`, `while`）的形式实现。
    *   **口诀**：先求解，后使用。

| 特性     | 递归 (Recursion)                 | 递推 (Iteration)                     |
| :------- | :------------------------------- | :----------------------------------- |
| **方向** | Top-Down (从大到小)              | Bottom-Up (从小到大)                 |
| **实现** | 函数调用自身                     | 循环                                 |
| **关键** | 递归出口 (Base Case)             | 初始状态 (Initial State)             |
| **优点** | 代码直观，易于理解和实现复杂逻辑 | 效率高，无函数调用开销，无栈溢出风险 |
| **缺点** | 函数调用开销大，可能导致栈溢出   | 代码可能不如递归直观，需明确计算顺序 |

## 二、递归三要素

编写一个正确的递归函数，必须明确以下三点：

1.  **函数定义**：明确函数的功能。例如，`fib(n)` 的功能是“计算斐波那契数列的第 `n` 项”。
2.  **递归关系**：找到大问题与子问题的关系。例如，`fib(n) = fib(n-1) + fib(n-2)`。
3.  **递归出口 (Base Case)**：定义问题最小规模的解，这是递归的终点。例如，`fib(0) = 0`, `fib(1) = 1`。

**示例：阶乘**
```cpp
// 递归实现阶乘
int factorial(int n) {
    // 1. 函数定义：计算 n 的阶乘
    // 3. 递归出口
    if (n == 0) {
        return 1;
    }
    // 2. 递归关系：n! = n * (n-1)!
    return n * factorial(n - 1);
}
```

## 三、递推与动态规划 (DP)

递推是动态规划最常见的实现方式。DP 的核心就是找到**状态**和**状态转移方程**。

*   **状态**：通常用 `dp[i]` 或 `dp[i][j]` 表示解决规模为 `i` (或 `i, j`) 的子问题时的最优解。
*   **状态转移方程**：即递推关系式，描述了状态之间如何演化。例如 `dp[i] = dp[i-1] + dp[i-2]`。

**示例：斐波那契数列**
```cpp
// 递推实现斐波那契数列
int fibonacci(int n) {
    if (n <= 1) return n;
    vector<int> dp(n + 1);
    // 初始状态
    dp[0] = 0;
    dp[1] = 1;
    // 递推关系
    for (int i = 2; i <= n; ++i) {
        dp[i] = dp[i - 1] + dp[i - 2];
    }
    return dp[n];
}
```

## 四、递归的优化：记忆化搜索

**问题**：朴素递归会重复计算大量相同的子问题（如 `fib(5)` 会多次计算 `fib(3)`），导致指数级时间复杂度。

**记忆化搜索 (Memoization)**：是**递归**和**动态规划**思想的完美结合。它在递归的基础上，增加一个“备忘录”（通常是数组或哈希表），用于存储已计算过的子问题的解。

*   **核心流程**：
    1.  在函数入口，检查备忘录中是否已有当前状态的解。
    2.  如果有，直接返回，避免重复计算。
    3.  如果没有，按正常递归逻辑计算。
    4.  在返回结果前，将解存入备忘录。

**示例：记忆化搜索求斐波那契**
```cpp
vector<int> memo; // 备忘录

int fib_memo(int n) {
    if (n <= 1) return n;
    // 检查备忘录
    if (memo[n] != -1) {
        return memo[n];
    }
    // 计算并存入备忘录
    memo[n] = fib_memo(n - 1) + fib_memo(n - 2);
    return memo[n];
}
```
**本质**：记忆化搜索是用递归的形式，实现了递推（DP）的效果。它在逻辑上是自顶向下的，但在计算顺序上，每个子问题仍然只被计算一次。这使得它兼具了递归代码的直观性和 DP 的高效率。


# 前缀和与差分核心笔记

## 一、核心思想：预处理与逆运算

前缀和（Prefix Sum）与差分（Difference Array）是一对互为**逆运算**的技巧。它们都利用**预处理**思想，将某些频繁的操作进行优化。

*   **前缀和**：通过预处理，将**多次区间查询**的复杂度从 `O(N)` 降至 `O(1)`。
*   **差分**：通过预处理，将**多次区间修改**的复杂度从 `O(N)` 降至 `O(1)`。

| 操作         | 朴素做法 | 优化技巧   | 预处理复杂度 | 操作复杂度 |
| :----------- | :------- | :--------- | :----------- | :--------- |
| **区间求和** | `O(N)`   | **前缀和** | `O(N)`       | `O(1)`     |
| **区间修改** | `O(N)`   | **差分**   | `O(N)`       | `O(1)`     |

## 二、前缀和 (Prefix Sum)

**核心思想**：预先计算出数组从开头到每一位的元素总和。用空间换时间。

#### 一维前缀和

*   **定义**：`pre[i]` 存储原数组 `A` 中 `A[1]` 到 `A[i]` 的总和。
*   **构造 (预处理)**：`pre[i] = pre[i-1] + A[i]`
*   **应用 (区间查询)**：计算 `A[L]` 到 `A[R]` 的和。
    *   **公式**：`sum(L, R) = pre[R] - pre[L-1]`
    *   **复杂度**：预处理 `O(N)`，每次查询 `O(1)`。

#### 二维前缀和

*   **定义**：`pre[i][j]` 存储以 `(1,1)` 为左上角，`(i,j)` 为右下角的矩形区域内所有元素的和。
*   **构造 (预处理)**：利用容斥原理。
    *   **公式**：`pre[i][j] = pre[i-1][j] + pre[i][j-1] - pre[i-1][j-1] + A[i][j]`
*   **应用 (矩形区域求和)**：计算以 `(x1, y1)` 为左上角，`(x2, y2)` 为右下角的矩形和。
    *   **公式**：`sum = pre[x2][y2] - pre[x1-1][y2] - pre[x2][y1-1] + pre[x1-1][y1-1]`
    *   **复杂度**：预处理 `O(N*M)`，每次查询 `O(1)`。

## 三、差分 (Difference Array)

**核心思想**：存储数组中相邻元素的差。对一个区间进行增减操作，只会影响到区间的两个端点在差分数组中对应的值。

#### 一维差分

*   **定义**：`diff[i]` 存储 `A[i] - A[i-1]` (规定 `A[0]=0`)。
    *   `diff[1] = A[1]`
    *   `diff[i] = A[i] - A[i-1]` for `i > 1`
*   **性质**：原数组 `A` 是差分数组 `diff` 的前缀和。`A[i] = pre_sum(diff, i)`。
*   **构造 (预处理)**：`diff[i] = A[i] - A[i-1]`
*   **应用 (区间修改)**：将原数组 `A` 的 `[L, R]` 区间内所有元素加上 `val`。
    *   **操作**：`diff[L] += val; diff[R+1] -= val;`
    *   **原理**：
        *   `diff[L] += val` 使得从 `A[L]` 开始的所有元素都增加了 `val`。
        *   `diff[R+1] -= val` 抵消了从 `A[R+1]` 开始的增加效果，从而保证只有 `[L, R]` 区间受到了影响。
    *   **复杂度**：预处理 `O(N)`，每次修改 `O(1)`。修改完成后，若需得到最终数组，再对差分数组求一次前缀和，复杂度 `O(N)`。

#### 二维差分

*   **思想**：与二维前缀和类似，`diff[i][j]` 的改变会影响其右下方所有区域。对一个矩形区域进行修改，只需在 4 个关键点进行操作。
*   **应用 (矩形区域修改)**：将以 `(x1, y1)` 为左上角，`(x2, y2)` 为右下角的矩形区域内所有元素加上 `val`。
    *   **操作**：
        ```
        diff[x1][y1] += val;
        diff[x1][y2+1] -= val;
        diff[x2+1][y1] -= val;
        diff[x2+1][y2+1] += val;
        ```
    *   **原理**：同样是容斥原理。在 `(x1, y1)` 增加 `val` 影响整个右下区域，再在另外三个角进行“减”和“加”操作来抵消多余的影响。

**总结**：前缀和与差分是处理静态数组区间问题的利器。当题目涉及大量**区间查询**时，考虑**前缀和**；当涉及大量**区间修改**时，考虑**差分**。它们是算法竞赛中必须熟练掌握的基础技巧。



# 二分查找 (Binary Search) 核心笔记

## 一、核心思想：单调性与对半舍弃

二分查找是一种在**有序序列**中进行查找的高效算法。其精髓在于利用序列的**单调性**，每次将搜索区间缩小一半。

*   **前提**：查找的数组、答案空间必须具有**单调性**或**可二分性**。这意味着我们可以通过检查中间点，明确地判断答案在左半部分还是右半部分。
*   **威力**：将查找时间复杂度从 `O(N)` 降至 `O(log N)`。

## 二、二分查找的两种类型

1.  **整数二分**：在整数集合（如数组下标）中查找。**细节最多，最易出错**。
2.  **实数二分**：在实数域上查找。逻辑相对简单，通过控制精度来终止。

## 三、整数二分：手写模板与细节剖析

整数二分的难点在于**边界处理**。`l`、`r`、`mid` 的取值和更新稍有不慎就会导致死循环或错过正确答案。


以数组 `A = [1, 2, 4, 5, 5, 5, 7, 9]` (0-based index) 为例，看似微小的表述差异，会导致结果截然不同：

| 查找目标                 | 期望索引    |
| :----------------------- | :---------- |
| 第一个 **>** 5 的元素    | `6` (值为7) |
| 第一个 **>=** 5 的元素   | `3` (值为5) |
| 最后一个 **<** 5 的元素  | `2` (值为4) |
| 最后一个 **<=** 5 的元素 | `5` (值为5) |

如果针对每种情况单独设计二分逻辑，不仅繁琐，而且极易因边界处理不当而出错。**需要一个更通用的抽象模型。**

#### 核心抽象：“红蓝染色”模型

与其纠结于 `>`、`>=`、`<`、`<=`，不如使用一个更通用的模型：

> 将有序序列抽象为两部分：一部分不满足 `check(x)` 条件（红色），另一部分满足 `check(x)` 条件（蓝色）。二分的目标就是找到**红蓝两区的分界点**。

这涵盖了所有整数二分问题。我们要做的就是确定：
1.  `check(mid)` 函数的含义是什么？（例如，`check(i)` 定义为 `A[i] >= 5`）
2.  我们要找的是 “蓝色” 的左边界，还是 “蓝色” 的右边界？

#### 实现思想：边界推进

维护两个指针 `l` 和 `r`，它们分别代表序列被划分成的左右两个区域的边界：

* **`l`**：左侧区域的**右端点**。
* **`r`**：右侧区域的**左端点**。

循环的核心是判断 `mid` 的颜色，并据此移动 `l` 或 `r`，从而扩张其中一个区域的边界，直至二者相遇。
当循环结束时，`l` 与 `r` 会合于目标蓝区的边界点。
因此，实际上：

* 一个指针维护的是 **蓝色区域的已确认边界**；
* 另一个指针维护的是 **红色区域的已确认边界向蓝色方向拓展 1 的位置**。


#### 模板 1: 寻找满足条件的最左值

该模板用于 `[红, 红, ..., 蓝, 蓝]` 模式，目标是找到**第一个**满足 `check(mid)` 的位置（即蓝区的左边界）。

在此情形下：

* `l` 表示**红色区域的端点向蓝色方向拓展 1 的位置**；
* `r` 表示**蓝色区域的端点**。
  通过 `l = mid + 1`，可确保最终 `l == r` 时，收束于蓝区的左边界。

```cpp
// 在闭区间 [L, R] 中查找第一个满足 check(x) 的 x
int binary_search_template_1(int L, int R) {
    int l = L, r = R;
    while (l < r) {
        int mid = l + r >> 1; // 向下取整
        if (check(mid)) {
            r = mid;          // mid 在蓝区，蓝色确认边界 [r] 更新为 [mid]
        } else {
            l = mid + 1;      // mid 在红区，红色确认边界+1 [l] 更新为 [mid+1]
        }
    }
    return l; // 或 r，循环结束时 l == r，位于蓝区左边界
}
```


#### 模板 2: 寻找满足条件的最右值

该模板用于 `[蓝, 蓝, ..., 红, 红]` 模式，目标是找到**最后一个**满足 `check(mid)` 的位置（即蓝区的右边界）。

在此情形下：

* `l` 表示**蓝色区域的端点**；
* `r` 表示**红色区域的端点向蓝色方向拓展 1 的位置**。
  通过 `r = mid - 1`，可确保最终 `l == r` 时，收束于蓝区的右边界。

```cpp
// 在闭区间 [L, R] 中查找最后一个满足 check(x) 的 x
int binary_search_template_2(int L, int R) {
    int l = L, r = R;
    while (l < r) {
        int mid = l + r + 1 >> 1; // 向上取整
        if (check(mid)) {
            l = mid;              // mid 在蓝区，蓝色确认边界 [l] 更新为 [mid]
        } else {
            r = mid - 1;          // mid 在红区，红色确认边界-1 [r] 更新为 [mid-1]
        }
    }
    return l; // 或 r，循环结束时 l == r，位于蓝区右边界
}
```

#### 关键步骤：验证返回结果

手写二分模板在找不到合法解时，会返回区间的边界。因此，**不能保证答案在区间内存在时，需要对返回值进行验证。**

```cpp
// 示例：使用模板2后进行验证
int ans = binary_search_template_2(L, R);
if (!check(ans)) {
    cout << "未找到满足条件的元素" << endl;
} else {
    cout << "最后一个满足条件的元素是：" << ans << endl;
}
```

#### 模板细节深度剖析

1.  **`while (l < r)`**：
    *   **含义**：只要区间长度大于1，就继续二分。
    *   **为什么不是 `l <= r`**：当 `l == r` 时，区间已经缩小到唯一的点，这个点就是答案，循环应该终止。如果使用 `l <= r`，在某些更新策略下（如 `l = mid`），当 `l` 和 `r` 相邻时可能导致死循环。`l < r` 是最安全的选择。

2.  **`mid` 的取整方式 (最关键的防死循环细节)**：
    *   **规则**：`mid` 的取整方式必须与边界收缩的方式相匹配，以确保区间总能缩小。
    *   **场景1：`r = mid`** (模板1)
        *   当区间只剩两个元素 `[l, l+1]` 时，`mid = (l + l+1) >> 1` 会得到 `l`。
        *   如果此时 `check(mid)` 为 `true`，`r` 会更新为 `mid` (`l`)，区间变为 `[l, l]`，循环终止。
        *   如果 `check(mid)` 为 `false`，`l` 会更新为 `mid+1` (`l+1`)，区间变为 `[l+1, l+1]`，循环终止。
        *   **结论**：`mid = l + r >> 1` (向下取整) 与 `r = mid` 搭配是安全的。
    *   **场景2：`l = mid`** (模板2)
        *   当区间只剩两个元素 `[l, l+1]` 时，如果用 `mid = l + r >> 1`，`mid` 仍为 `l`。
        *   如果此时 `check(mid)` 为 `true`，`l` 更新为 `mid` (`l`)，区间仍是 `[l, l+1]`，**发生死循环！**
        *   **解决方案**：必须向上取整！`mid = (l + r + 1) >> 1`。这样在 `[l, l+1]` 时，`mid` 会得到 `l+1`，确保区间能缩小。
    *   **记忆口诀**：更新 `l = mid` 时，`mid` 必须向上取整 (`+1`)。

3.  **边界更新 `+1` 或 `-1`**：
    *   如果 `check(mid)` 满足条件，而我们要找的是**第一个**满足条件的，那么 `mid` 本身就是一个潜在的答案，所以我们收缩右边界时不能排除它：`r = mid`。
    *   如果 `check(mid)` 不满足条件，那么 `mid` 肯定不是答案，可以直接排除：`l = mid + 1` 或 `r = mid - 1`。


## 四、STL 中的二分查找函数 (`lower_bound` / `upper_bound`)

C++ 标准库 `<algorithm>` 提供了两个强大的、经过优化的二分查找函数，可以直接在**已排序**的容器（如 `vector`, `array`）或数组上使用。它们返回的是**迭代器**。

#### `lower_bound`

*   **功能**：查找**第一个大于或等于 (`>=`)**给定值的元素。
*   **与模板的联系**：这完全等价于我们的**模板 1**，其中 `check(x)` 的定义是 `x >= val`。它寻找的是 `[false, false, ..., true, true, ...]` 分割线中第一个 `true` 的位置。
*   **用法**：`lower_bound(begin, end, val)`
*   **返回值**：
    *   如果找到，返回指向该元素的迭代器。
    *   如果找不到（即所有元素都小于 `val`），返回 `end` 迭代器。

#### `upper_bound`

*   **功能**：查找**第一个严格大于 (`>`)**给定值的元素。
*   **与模板的联系**：这同样可以看作是**模板 1** 的应用，其中 `check(x)` 的定义是 `x > val`。
*   **用法**：`upper_bound(begin, end, val)`
*   **返回值**：
    *   如果找到，返回指向该元素的迭代器。
    *   如果找不到（即所有元素都小于或等于 `val`），返回 `end` 迭代器。

#### 实用技巧与代码示例

假设有一个已排序的 `vector<int> v = {10, 20, 30, 30, 40, 50};`

1.  **获取索引**：用返回的迭代器减去起始迭代器 `v.begin()`。
2.  **查找 `>= 30` 的第一个元素**：
    ```cpp
    auto it = lower_bound(v.begin(), v.end(), 30);
    // it 指向索引为 2 的 30
    int index = it - v.begin(); // index = 2
    ```
3.  **查找 `> 30` 的第一个元素**：
    ```cpp
    auto it = upper_bound(v.begin(), v.end(), 30);
    // it 指向索引为 4 的 40
    int index = it - v.begin(); // index = 4
    ```
4.  **查找 `== 30` 的最后一个元素**：
    `upper_bound` 找到第一个大于 `30` 的位置，其前一个位置就是最后一个 `<= 30` 的元素。如果该元素恰好是 `30`，就找到了。
    ```cpp
    auto it = upper_bound(v.begin(), v.end(), 30);
    it--; // 指向索引为 3 的 30
    int index = it - v.begin(); // index = 3
    ```
5.  **计算等于 `val` 的元素个数**：
    `upper_bound` 的位置减去 `lower_bound` 的位置，就是等于 `val` 的元素区间长度。
    ```cpp
    auto low = lower_bound(v.begin(), v.end(), 30);
    auto up = upper_bound(v.begin(), v.end(), 30);
    int count = up - low; // count = 2
    ```
6.  **判断元素是否存在**：
    ```cpp
    auto it = lower_bound(v.begin(), v.end(), 35);
    // it != v.end() 检查是否越界
    // *it == 35 检查找到的是否就是目标值
    if (it != v.end() && *it == 35) {
        // 存在
    } else {
        // 不存在
    }
    ```

**何时使用手写模板，何时使用 STL？**

*   **使用 STL (`lower_bound`/`upper_bound`)**：当你在一个**已排序的数组或容器**中，进行**简单的值查找**时（如 `==`, `>=`, `>`)。它代码简洁、不易出错。
*   **使用手写二分模板**：当二分的对象不是一个具体的数组，而是**答案空间**时（例如，求解“最大值的最小值”问题）。这时你需要自定义 `check` 函数的复杂逻辑，手写模板提供了必要的灵活性。


## 五、实数二分

实数二分逻辑更简单，因为不需要处理恼人的整数边界。

*   **终止条件**：不再是 `l < r`，而是通过**精度**或**固定次数**来控制。
    *   **精度控制**：`while (r - l > eps)`，其中 `eps` 是一个极小值 (如 `1e-7`, `1e-8`)。
    *   **次数控制**：`for (int i = 0; i < 100; ++i)`。对于 `double` 类型，循环 100 次足以达到非常高的精度。

#### 实数二分模板

```cpp
double binary_search_real(double L, double R) {
    const double eps = 1e-8;
    // while (R - L > eps) { // 写法1：精度控制
    for (int i = 0; i < 100; ++i) { // 写法2：次数控制，更常用
        double mid = L + (R - L) / 2; // 避免溢出，且实数无取整问题
        if (check(mid)) {
            R = mid; // 或 L = mid，取决于 check 的定义
        } else {
            L = mid;
        }
    }
    return L; // 或 R，两者非常接近
}
```

## 总结

掌握“红蓝染色”模型，并牢记两个整数二分模板及其背后的防死循环原理，是彻底征服**答案空间二分**的关键。对于**数组上的值查找**，应优先使用 `lower_bound` 和 `upper_bound`，它们更简洁、更安全。对于实数二分，则关注精度控制即可。

