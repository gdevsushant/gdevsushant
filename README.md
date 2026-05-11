<div align="center">

# Hi, I'm Sushant 👋  
### Unreal Engine Systems Developer | Gameplay Architecture | Plugin Developer

I build scalable Unreal Engine systems, gameplay frameworks, editor tools, and reusable C++ plugins.

</div>

---

## 🧠 About Me

I am focused on **Unreal Engine C++ development**, especially:

- Gameplay systems architecture
- Modular weapon systems
- Runtime plugin development
- Blueprint + C++ framework design
- Serialization systems
- GameplayTag-based communication systems
- Editor tooling and reusable systems

My goal is to build production-style Unreal Engine systems that are clean, scalable, and easy to extend.

---

## 🚀 Featured Work

### 🔹 Dynamic Storage System
A runtime data storage plugin for Unreal Engine using Gameplay Tags as keys.

**Core Features**
- Generic C++ template API
- Blueprint support
- Primitive, struct, object, array, set, and map storage
- Runtime serialization
- Plugin-style architecture

```cpp
UDynamicStorageSystemAPI::SetValue<float>(
    this,
    FGameplayTag::RequestGameplayTag("Weapon.Scope.DefaultFOV"),
    85.0f
);

float FOV = UDynamicStorageSystemAPI::GetValue<float>(
    this,
    FGameplayTag::RequestGameplayTag("Weapon.Scope.DefaultFOV")
);
