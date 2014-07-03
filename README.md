# Module Documentation

## Module Data.List

### Types

    data List a where
      Nil :: List a
      Cons :: a -> List a -> List a


### Type Class Instances

    instance alternativeList :: Alternative List

    instance applicativeList :: Applicative List

    instance applyList :: Apply List

    instance bindList :: Bind List

    instance eqList :: (Eq a) => Eq (List a)

    instance foldableList :: Foldable List

    instance functorList :: Functor List

    instance monadList :: Monad List

    instance monoidList :: Monoid (List a)

    instance ordList :: (Ord a) => Ord (List a)

    instance semigroupList :: Semigroup (List a)

    instance showList :: (Show a) => Show (List a)

    instance traversableList :: Traversable List


### Values

    (!) :: forall a. List a -> Number -> Maybe a

    catMaybes :: forall a. List (Maybe a) -> List a

    drop :: forall a. Number -> List a -> List a

    filter :: forall a. (a -> Boolean) -> List a -> List a

    fromArray :: forall a. [a] -> List a

    length :: forall a. List a -> Number

    mapMaybe :: forall a b. (a -> Maybe b) -> List a -> List b

    take :: forall a. Number -> List a -> List a

    toArray :: forall a. List a -> [a]