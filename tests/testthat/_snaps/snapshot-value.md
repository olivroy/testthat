# can snapshot values

    [
      "a",
      1.5,
      1,
      true
    ]

---

    {
      "type": "list",
      "attributes": {},
      "value": [
        {
          "type": "character",
          "attributes": {},
          "value": ["a"]
        },
        {
          "type": "double",
          "attributes": {},
          "value": [1.5]
        },
        {
          "type": "integer",
          "attributes": {},
          "value": [1]
        },
        {
          "type": "logical",
          "attributes": {},
          "value": [true]
        }
      ]
    }

---

    list("a", 1.5, 1L, TRUE)

---

    WAoAAAACAAQCAwACAwAAAAATAAAABAAAABAAAAABAAQACQAAAAFhAAAADgAAAAE/+AAAAAAA
    AAAAAA0AAAABAAAAAQAAAAoAAAABAAAAAQ==

# can control snapshot value details

    1.2

# tolerance passed to check_roundtrip

    0.9

# check_roundtrip() gives nice error

    Code
      wrapper(NULL, list(), label = "foo", style = "json")
    Condition
      Error in `wrapper()`:
      ! `foo` could not be safely serialized with `style = "json"`.
        Serializing then deserializing the object returned something new:
      
      `original` is NULL
      `new` is a list
      
      i You may need to try a different `style`.

