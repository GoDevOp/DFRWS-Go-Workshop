# Lab 1 – Windows FILETIME

## Table of Contents

* [Description](#desc)
* [References](#ref)

## Description <a name="desc"/>

In Windows, a `FILETIME` is a 64-bit value that represents the number of 100-nanosecond intervals that have elapsed since 12:00 A.M. January 1, 1601 Coordinated Universal Time (UTC).

In Go, a `time.Time` represents an instant in time with nanosecond precision.

In this lab you will create a new package called `time`, which contains the following defined `FileTime` type.  You must implement all method as defined by the documentation below.

#### type FileTime

```go
type FileTime int64
```

FileTime is a 64-bit value that represents the number of 100-nanosecond
intervals that have elapsed since 12:00 A.M. January 1, 1601 Coordinated
Universal Time (UTC).

#### func (FileTime) Time

```go
func (t FileTime) Time() time.Time
```
Time returns t as a standard time.Time

## References <a name="ref"/>

* [File Times (Windows) - MSDN - Microsoft](https://msdn.microsoft.com/en-us/library/windows/desktop/ms724290(v=vs.85).aspx)
* [time - The Go Programming Language](https://golang.org/pkg/time/)
