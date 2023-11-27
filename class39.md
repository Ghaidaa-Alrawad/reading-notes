# Class 39

1. What are the benefits and downfalls of using the ‘getLastLocation()’ method to get your device’s location?

The 'getLastLocation()' method in the fused location provider offers a quick way to retrieve a device's location, minimizing battery usage attributed to the app. However, it may provide outdated information if no other clients have actively used location recently. The downfall lies in the potential for less accurate or stale data.

---

2. What about the ‘getCurrentLocation()’ method?

On the other hand, the 'getCurrentLocation()' method aims for a fresher and more accurate location consistently. While it provides up-to-date information, it may cause active location computation, leading to higher battery consumption. It is recommended for obtaining a fresh location whenever possible but requires careful management to avoid excessive power usage, especially when compared to alternatives like 'requestLocationUpdates()'.

---

## Things I want to know more about 

The impact of Location Provider Usage