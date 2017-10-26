# Models / Enums

In alphabetical order are all the models with public properties (all properties can be viewed in [GitHub](https://github.com/Templarian/MaterialDesign-Site/tree/master/src/app/shared/models)).

## Models

```typescript
class Alias {
    public id: string,
    public name: string
}
```

```typescript
class Icon {
    public id: string;
    public name: string;
    public data: string;
    public user: User;
    public aliases: Alias[];
}
```

```typescript
class Modification {
    public id: string;
    public modificaitonId: ModificationType;
    public packageId: string;
    public user: User;
    public icon: Icon;
    public iconNameBefore: string;
    public iconNameAfter: string;
    public iconDataBefore: string;
    public iconDataAfter: string;
    public text: string;
    public date: Date;
    public issue: number;
}
```

```typescript
class Package {
    public name: string;
    public width: number;
    public height: number;
    public icons: Icon[];
}
```

```typescript
class Tag {
    public id: string;
    public name: string;
}
```

```typescript
class User {
    public id: string;
    public github: string;
    public twitter: string;
    public name: string;
    public base64: string;
}
```

## Enums

```typescript
enum ModificationType {
    AliasCreated = "691c8829-b1e7-11e7-bf5c-94188269ec50",
    IconCreated = "AFFE875E-01BC-4A34-9BE3-27625A155B28",
    IconDeleted = "B1CE1713-A18A-4E9D-9E26-D0B4E44A1FAC",
    IconModified = "1506F66B-CC2A-4575-A20A-DC138628977A",
    IconRenamed = "F7B6D49B-A86F-49AC-AF92-6B9D0DF6188B",
    WebfontPublished = "66B9FA99-1FAA-4D8F-B87F-B6F3CA444624",
    News = "B4DEB3A8-A146-4086-9D7B-B67842A9CCB8"
}
```