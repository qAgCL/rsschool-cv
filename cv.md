# Git-Markdown-Task in RSSchools
## Zahar Rubanov
## Contact info:
    agcl3228@gmail.com
    +375-29-367-52-07
    [VKontakte] (https://vk.com/qagcl)
    [Instagram] (https://www.instagram.com/qagcl/)
## Summary
My goal is to become a **full-stack developer**. At the moment, I'm learning *web-design* and *frontend development*. I'm trying to learn more about JS.

## Skills
I had programming experience in such languages as: *C, Assembler, C++, C#*. I'm pretty good at *C# .Net 5*.

## CodeExamples
```cs
public sealed class Segment
    {
        public int Left { get; }
        public int Right { get; }
        public uint Length => (uint)(Right - Left);
        public Segment(int a, int b)
        {
            if (a > b)
            {
                (a, b) = (b, a);
            }

            Left = a;
            Right = b;
        }

        public static implicit operator uint(Segment segment)
        {
            if (segment == null)
            {
                throw new ArgumentNullException(nameof(segment));
            }

            return segment.Length;
        }

        public static explicit operator Segment((int a, int b) tuple) => new Segment(tuple.a, tuple.b);
        public static Segment operator +(Segment s1, Segment s2)
        {
            if (s1 == null || s2 == null) throw new ArgumentNullException();
            return new Segment(s1.Left + s2.Left, s1.Right + s2.Right);
        }

        public override bool Equals(object obj) => obj is Segment segment && Length == segment.Length;

        public override int GetHashCode() => Length.GetHashCode();

        public override string ToString() => $"[{Left},{Right}]";
    }
```

## Education
I'm the third-year student of BSUIR.
Styding IsSoft C# developer school.

## English
Have a B1-level.
