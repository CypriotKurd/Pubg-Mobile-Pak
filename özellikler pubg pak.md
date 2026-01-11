#### **BASE\_PART**



* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Ana harita modelleri (Erangel/Primewood binalar, terrain), base textures (çimen, toprak LOD), skybox, lighting (sky sphere, post-process volumes). /Game/Maps/, /Game/Environment/



* ###### ***Fizik Özellikler (Collision/Physics/Ragdoll)***



Ana collision mesh'ler (duvar/yer çarpışma), terrain physics (slope walking), vehicle base collision. PhysicsAsset'ler (/Game/Physics/).



* ###### ***Diğer İçerikler (Ses/Config/Blueprint)***



Base blueprint'ler (player pawn base), config dosyaları (default.ini'ler).



* ###### ***Mod Tavsiyesi (Ne Değiştir?)***



Gökyüzü rengi (/Game/Maps/Common/Sky/), çimen görünmez yap (LOD bias). Fizik: Yer sürtünmesi arttır (Friction 1.2 → 1.5).







### **core\_patch**





* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Güncelleme textures (yeni skin'ler, weapon camo), particle effects base (ateş, duman). /Game/Effects/Core/, /Game/Materials/



* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Core physics update'ler (yeni weapon ragdoll, player fall damage anims). SkeletalMesh PhysicsData.



* ###### ***Diğer İçerikler (Ses/Config/Blueprint)***



Core lib'ler (libUE4.so referans), anti-cheat config'ler (ama client), DataTable'lar (base stats).



* ###### ***Mod Tavsiyesi (Ne Değiştir?)***



Duman rengi mor yap (/Game/Effects/Core/Smoke\_Niagara Color: 0.7,0,1). Fizik: Jump height client anim (AnimBP Curve 1.1 → 1.3).







#### **game\_patch**



* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Oyun modu asset'leri (Primewood harita objeleri, event effects), weapon models/textures. /Game/GameModes/, /Game/Weapons/



* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Silah/araç physics patch'leri (recoil anim client-side, vehicle flip physics). Chaos Physics (UE5) collision.



* ###### ***Diğer İçerikler (Ses/Config/Blueprint)***



Oyun blueprint'leri (match start/end), server sync config'ler (client prediction). Anti-cheat flag'ler burda.



* ###### ***Mod Tavsiyesi (Ne Değiştir?)***



Mermi izi rengi (/Game/Weapons/Effects/Tracer\_Mat Emissive: neon). Fizik: Araç hız client feel (WheelSetup MaxSpeed 100 → 120).







#### **res\_audio**



* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Yok (audio odaklı).



* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Yok.



* ###### ***Diğer İçerikler (Ses/Config/Blueprint)***



Tamamı ses: WWise .bnk/.wem dosyaları (silah sesi, ayak sesi, müzik, VO). /Game/Sounds/ altında SoundWave'ler.



* ###### ***Mod Tavsiyesi (Ne Değiştir?)***



Sesleri değiştir (silah sesi yüksek yap, .wem edit tool'la). Fizik etkilemez.









#### **res\_avatarko**





* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Kore region avatar skin'leri (yeni outfit textures, face/hair materials). /Game/Characters/AvatarKO/, HD textures.



* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Avatar skeletal mesh collision (body hitbox'lar), anim physics (dance emote ragdoll).



* ###### ***Diğer İçerikler (Ses/Config/Blueprint)***



Avatar blueprint'ler (customization), KO-specific DataTable'lar (skin stats client).



* ###### ***Mod Tavsiyesi (Ne Değiştir?)***



Skin rengi değiştir (Material Instance Color tint). Fizik: Emote anim hızı (AnimMontage Rate 1.0 → 1.5).









#### **res\_basetexmd**





* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Medium Detail (MD) base textures: Orta kaliteli textures (yakın mesafe: skin detay, weapon inspect). /Game/Textures/MD/.



* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



MD collision proxies (silah tutuş physics).



* ###### ***Diğer İçerikler (Ses/Config/Blueprint)***



Material instances MD LOD.



* ###### ***Mod Tavsiyesi (Ne Değiştir?)***



Skin parlaklık arttır (Roughness 0.4 → 0.2). Fizik: Tutuş anim smooth (IK bone scale).











#### **res\_es3shader**





* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Shader kaynakları: OpenGL ES3 shaders (mobile lighting, shadow maps, PBR materials). /Game/Shaders/ES3/.



* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Physics visualization shaders (wireframe collision debug).



* ###### ***Diğer İçerikler (Ses/Config/Blueprint)***



Vertex/Pixel shaders, compute shaders (particle sim).



* ###### ***Mod Tavsiyesi (Ne Değiştir?)***



Shader tweak: Glow efekti arttır (Emissive boost). Fizik: Collision glow (debug mode).









#### **res\_pufferpatch**







* ###### **<i>Görsel Özellikler (Textures/Materials/Effects)</i>**



Puffer compression patch: UE5 yeni texture compression (DTF format) için patch textures (yüksek kaliteli yeni asset'ler: Primewood foliage, water). /Game/Textures/Puffer/.



* ###### ***Görsel Özellikler (Textures/Materials/Effects)***



Puffer physics assets (optimized collision meshes, low mem ragdoll).



* ###### ***Diğer İçerikler (Ses/Config/Blueprint)***



Patch blueprint'ler (yeni compression loader), config (PufferCodec settings).



* ###### ***Mod Tavsiyesi (Ne Değiştir?)***



Toz/water rengi (/Game/Environment/Puffer\_Mat). Fizik: Yeni objelerde sürtünme (Puffer PhysicsAsset Damping).



