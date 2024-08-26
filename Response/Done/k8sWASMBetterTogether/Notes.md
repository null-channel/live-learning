article: https://thenewstack.io/webassembly-and-kubernetes-go-better-together-matt-butcher/

What does WASM solve that containers do not?
 - More secure? (maybe if each process has it's own WASM runtime, maybe per customer runtime?) is it secure enough?
 - Startup time? - not sure on this one, I think if each process runs in it's own WASM runtime this would be slower then a container, if in the same runtime lacking isolation, could it be faster then a container. Probably depends a lot on the container, but most of mine start in under 5 seconds so is this a big deal?

WASM Cons:
 - Lack of language support? if you write rust, golang, dart, python, java, kotlin, javascrit or c/c++ it's fine, else you are screwed.
 - requirement to transpile your code for production?
 - your code only runs in WASM now.
 - still sucks to debug
 - lacks good debuging, build and testing tooling - still (transpiling issue? not sure, it feels like typescript.)
 - Supports python and javascript


WASM Pros:
- Lacks PHP support
- lacks fortran support
- lacks R support

other alternatives?
![[Pasted image 20240524113202.png]]



What does chat gpt think (statistical analysis of the internet effectively)
```
Performance: Wasm is designed for high performance. It allows code to run at near-native speed by taking advantage of common hardware capabilities. This makes it ideal for compute-intensive applications like games, graphics, and simulations.

Language Agnostic: Wasm is not tied to any specific programming language. Developers can write code in languages like C, C++, Rust, and more, and compile it to WebAssembly. This flexibility allows leveraging existing codebases and skills.

Security: WebAssembly operates in a sandboxed environment, which provides a robust security model. This helps in preventing unauthorized access and reduces the risk of exploits, making it safer to run untrusted code.

Portability: Wasm is designed to be portable across different environments. It can run on various platforms and devices, including desktops, mobile devices, and IoT devices, without modification.

Size and Load Time: Wasm modules are typically smaller in size compared to traditional JavaScript, leading to faster download and quicker execution. This improves the overall user experience, especially in scenarios with limited bandwidth.

Interoperability with JavaScript: Wasm can interoperate seamlessly with JavaScript. Developers can call WebAssembly functions from JavaScript and vice versa, allowing gradual adoption and integration into existing web applications.
sandboxing
Tooling and Ecosystem: The WebAssembly ecosystem is rapidly growing, with robust tooling, libraries, and frameworks supporting development. This includes support from major browsers and contributions from the open-source community.

Future-Proofing: With broad industry support and ongoing standardization, Wasm is set to play a significant role in the future of web development. Investing in WebAssembly skills and technologies can help future-proof applications.
```

Runtimes seem inmature in my opinion?

maybe the best one I know of is:
https://github.com/wasmerio/wasmer

But I still am hard pressed to understand running this in "un-trusted multi-tenet" mode and if I can't do that I don't understand how it would solve any problem a container does not solve better?