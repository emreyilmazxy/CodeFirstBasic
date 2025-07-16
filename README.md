# PatikaFirstDb EF Core Projesi

Bu proje, .NET 8 ile Entity Framework Core (Code First) kullanılarak geliştirilmiştir. Proje kapsamında PostgreSQL veritabanı ile `Movies` ve `Games` tabloları oluşturulmuştur.

## 📦 Özellikler

- Code First yaklaşımı ile veritabanı oluşturma
- Fluent API ile tablo yapılandırması
- PostgreSQL bağlantısı (Npgsql)
- EF Core `Migrations` kullanımı

## 📋 Tablolar

### 🎬 Movies
- `Id` (int, PK)
- `Title` (string, max 200)
- `Genre` (string, max 50)
- `ReleaseYear` (int)

### 🎮 Games
- `Id` (int, PK)
- `Name` (string, max 100)
- `Platform` (string, max 50)
- `Rating` (decimal, 0.0 – 10.0)

## ⚙️ Kullanılan Teknolojiler
- .NET 6
- Entity Framework Core
- PostgreSQL
- Npgsql.EntityFrameworkCore.PostgreSQL

## 🚀 Migration Komutları

```bash
dotnet ef migrations add InitialCreate
dotnet ef database update
