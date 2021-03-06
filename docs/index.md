# pinax-testimonials


!!! note "Pinax Ecosystem"
    This app is part of the Pinax ecosystem and is designed for use
    both with and independently of other Pinax apps.

    To learn more about Pinax, see <http://pinaxproject.com/>


## Quickstart

To install pinax-testimonials:

    pip install pinax-testimonials

Add `pinax-testimonials` to your `INSTALLED_APPS` setting:

    INSTALLED_APPS = (
        ...
        "pinax.testimonials",
        ...
    )

## Usage

In your template where you want to display testimonials there are three ways you
can use template tags to add active testimonials to your page.

First, load the template tags:

    {% load pinax_testimonials_tags %}


For random testimonials:

    {% random_testimonials <number> as quotes %}


For testimonials ordered by the date they were added:

    {% testimonials <number> as quotes %}


If you just want a single random testimonial you can use:

    {% random_testimonial as quote %}


Add and manage testimonial quotes via the Django admin.

## Changelog

See [Changelog](./changelog.md).