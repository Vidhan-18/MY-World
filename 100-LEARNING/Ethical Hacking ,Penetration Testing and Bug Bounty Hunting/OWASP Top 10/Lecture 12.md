# **Insecure Deserialization** 
- Applications those serialize **hostile or tampered object by attacker.**
- **When an application serializes and deserialize the data based on input without checking it properly may lead ==RCE==
# Why ID Happens
- Accept serialized objects from untrusted source an deserialize it.
# **What can be achieved by ID?**
- RCE
- Sensitive files disclosure==(/etc/passed)==
# **How do we fix issues** 
- Best way is **not to accept** serialized objects from untrusted sources.
- **Integrity checks** for serialized objects to prevent hostile object creation or data tempering.
- **Logging** deserialization exception and failures, such as where the incoming type is not the expected type, or the deserialization throws exceptions.